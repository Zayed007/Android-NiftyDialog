# Android-NiftyDialog

```
final NiftyDialogBuilder dialogBuilder = NiftyDialogBuilder.getInstance(getActivity());

dialogBuilder
                .withTitle(null)
                .withTitleColor(com.genericslab.droidplate.R.color.white)
                .withMessage("You have not completed your package.Are you sure to complete the Package and send SMS?")
                .withMessageColor("#FFFFFF")
                .withDialogColor("#03A9F4")
                .withDuration(100)
                .withEffect(Effectstype.Fadein)
                .isCancelableOnTouchOutside(false)
                .withButton1Text(getActivity().getResources().getString(android.R.string.ok))
                .withButton2Text(getActivity().getResources().getString(android.R.string.cancel))
                .setButton1Click(new View.OnClickListener() {
                    @Override
                    public void onClick(View view) {
                    
                    //
                    // do your code here
                    // 
                        
                        dialogBuilder.cancel();
                    }
                })
                .setButton2Click(new View.OnClickListener() {
                    @Override
                    public void onClick(View view) {
                        dialogBuilder.cancel();
                    }
                })
                .show();
```
