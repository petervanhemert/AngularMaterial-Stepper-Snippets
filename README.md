# AngularMaterial-Stepper-Snippets
Stepper code snippets


Disable mat-step header button
Add this to your main style sheet. It should be at the parent level so it can be overwritten
.mat-horizontal-stepper-header{
    pointer-events: none !important;
}
and set the tabindex attributes of the stepper-headers to '-1'
 <mat-step [stepControl]="frmStepOne" [attr.tabindex]="-1">
so you can't tab to the steps with a keyboard
