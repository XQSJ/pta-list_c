# pta-list_c
pta的c语言顺序表题目答案
#ifndef _LElement_h_
#define _LElement_h_

#include "Real.h"

typedef double LELEMENT;

void LElementInput(LELEMENT *x);
void LElementOutput(const LELEMENT *x);

int LElementGt(const LELEMENT *x, const LELEMENT *y);
int LElementGe(const LELEMENT *x, const LELEMENT *y);
int LElementLt(const LELEMENT *x, const LELEMENT *y);
int LElementLe(const LELEMENT *x, const LELEMENT *y);
int LElementEq(const LELEMENT *x, const LELEMENT *y);
nt LElementNe(const LELEMENT *x, const LELEMENT *y);

void LElementSwap(LELEMENT *x, LELEMENT *y);
说明：参数 `x` 和 `y` 为指示两个数据元素的指针。

- LELEMENT 为线性表的数据元素类型。

- LElementInput 输入数据元素。

- 输入数据元素到指针 `x` 所指示的变量中。

- LElementOutput 输出数据元素。

- 输出指针 `x` 所指数据元素的值。

- LElementGt、LElementGe、LElementLt、LElementLe、LElementEq 和 LElementNe 用于比较两个数据元素的值（要求：当两个实数非常接近，即：$$\mid x - y \mid < \epsilon$$ 时，认为它们相等）。

- 若 `x` 所指数据元素大于 `y` 所指数据元素，则 LElementGt 函数值为 1(真)，否则为 0(假)。
- 若 `x` 所指数据元素大于等于 `y` 所指数据元素，则 LElementGe 函数值为 1(真)，否则为 0(假)。
- 若 `x` 所指数据元素小于 `y` 所指数据元素，则 LElementLt 函数值为 1(真)，否则为 0(假)。
- 若 `x` 所指数据元素小于等于 `y` 所指数据元素，则 LElementLe 函数值为 1(真)，否则为 0(假)。
- 若 `x` 所指数据元素等于 `y` 所指数据元素，则 LElementEq 函数值为 1(真)，否则为 0(假)。
- 若 `x` 所指数据元素不等于 `y` 所指数据元素，则 LElementNe 函数值为 1(真)，否则为 0(假)。
- LElementSwap 交换数据元素的值。
