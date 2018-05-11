## Angular Vue 同义词汇表

这里是 Angular 而不是 AngularJS，AngularJS 指 1.x 版本

| Angular                                                                                                                          | Vue                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `{{}}`                                                                                                                           | `{{}}`                                                                    |
| `<p title="{{msg}}"></p>`                                                                                                        | `<p :title="msg"></p>`                                                    |
| `<p [title]="msg"></p>`                                                                                                          | `<p :title="msg"></p>`                                                    |
| `<p [innerHTML]="html"></p>`                                                                                                     | `<p v-html="html"></p>`                                                   |
| `<p *ngFor="let item of list;let key = index"></p>`                                                                              | `<p v-if="value,key in list"></p>`                                        |
| `<p template="ngFor let item of list;let key = index"></p>`                                                                      | `<p v-if="value,key in list"></p>`                                        |
| `<p (click)="fn()"></p>`                                                                                                         | `<p @click="fn"></p>`                                                     |
| `<input [(ngModel)]="model" />`( 需要引入 FormsModuel)                                                                           | `<input v-model="model" />`                                               |
| `<p *ngIf="boolean"></p>`                                                                                                        | `<p v-if="boolean"></p>`                                                  |
| `<div *ngIf="num; then num2; else num3">1</div>`<br>`<ng-template #num2>2</ng-template>`<br>`<ng-template #num3>3</ng-template>` | `<p v-if="num">1</p>`<br>`<p v-if-else="num2">2</p>`<br>`<p v-else>3</p>` |
