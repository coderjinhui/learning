## Angular Vue 同义词汇表

这里是 Angular 而不是 AngularJS，AngularJS 指 1.x 版本<br>
用来记录两者相似命令，方法等，方便自己记忆，当然更多的是方便自己能速查，因为自己会 Vue，因此做完对照表就能在查完 Angular 后能知道是怎么用、有何用处

| Angular                                                                                                                          | Vue                                                                          |
| -------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `{{}}`                                                                                                                           | `{{}}`                                                                       |
| `<p title="{{msg}}"></p>`                                                                                                        | `<p :title="msg"></p>`                                                       |
| `<p [title]="msg"></p>`                                                                                                          | `<p :title="msg"></p>`                                                       |
| `<p [innerHTML]="html"></p>`                                                                                                     | `<p v-html="html"></p>`                                                      |
| `<p *ngFor="let item of list;let key = index"></p>`                                                                              | `<p v-for="value,key in list"></p>`                                          |
| `<p template="ngFor let item of list;let key = index"></p>`                                                                      | `<p v-for="value,key in list"></p>`                                          |
| `<p (click)="fn()"></p>`                                                                                                         | `<p @click="fn"></p>`                                                        |
| `<input [(ngModel)]="model" />`( 需要引入 FormsModuel)                                                                           | `<input v-model="model" />`                                                  |
| `<p *ngIf="boolean"></p>`                                                                                                        | `<p v-if="boolean"></p>`                                                     |
| `<div *ngIf="num; then num2; else num3">1</div>`<br>`<ng-template #num2>2</ng-template>`<br>`<ng-template #num3>3</ng-template>` | `<p v-if="num">1</p>`<br>`<p v-if-else="num2">2</p>`<br>`<p v-else>3</p>`    |
| `<child [msg]="message"></child>`<br>in child:<br>`@Input() msg;`                                                                | `<child :msg="message"></child>`<br>in child:<br>`props: ['msg']`            |
| `<child (parent)="fn"></child>`<br>in child:<br>`@Output() parent=new EventEmitter()`<br>`this.parent.emit("data")`              | `<child @parent="fn"></child>`<br>in child:<br>`this.$emit('parent','data')` |
