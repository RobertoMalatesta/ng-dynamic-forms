# NG Dynamic Forms Basic UI

## Installation
```
npm install @ng-dynamic-forms/ui-basic -S
```

## Import
```ts
@NgModule({

    imports: [
        // ...
        ReactiveFormsModule,
        DynamicFormsCoreModule.forRoot(),
        DynamicFormsBasicUIModule
    ]
})

export class AppModule {}
```

## Usage

with **`DynamicBasicFormComponent`**:
```ts
<form [formGroup]="myFormGroup">

    <dynamic-basic-form [group]="myFormGroup"
                        [model]="myFormModel"></dynamic-basic-form>
</form>
```

with **`DynamicBasicFormControlComponent`**:
```ts
<form [formGroup]="myFormGroup">

    <dynamic-basic-form-control *ngFor="let controlModel of myFormModel"
                                [group]="myFormGroup"
                                [model]="controlModel"></dynamic-basic-form-control>
</form>
```

## Form Controls

|                                   Control                                  	|            Model            	| Required Property 	|
|:--------------------------------------------------------------------------:	|:---------------------------:	|:-----------------:	|
|    **[Checkbox](https://www.w3.org/wiki/HTML/Elements/input/checkbox)**    	|    `DynamicCheckboxModel`   	|         –         	|
| **[Checkbox Group](https://www.w3.org/wiki/HTML/Elements/input/checkbox)** 	| `DynamicCheckboxGroupModel` 	|         –         	|
|          **[Input](https://www.w3.org/wiki/HTML/Elements/input)**          	|     `DynamicInputModel`     	|         –         	|
|    **[Radio Group](https://www.w3.org/wiki/HTML/Elements/input/radio)**    	|   `DynamicRadioGroupModel`  	|         –         	|
|         **[Select](https://www.w3.org/wiki/HTML/Elements/select)**         	|     `DynamicSelectModel`    	|         –         	|
|       **[TextArea](https://www.w3.org/wiki/HTML/Elements/textarea)**       	|    `DynamicTextAreaModel`   	|         –         	|

## Sample

[**Live Demo**](http://ng2-dynamic-forms.udos86.de/sample/index.aot.html#basic-sample-form) 