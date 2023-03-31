#include <stdio.h>
#include <stdlib.h>
#include <ctype.h>  // 提供isdigit函数

#define MAX_SIZE 100  // 定义栈的最大容量

typedef struct {
    int data[MAX_SIZE];
    int top;  // 栈顶指针
} Stack;

// 初始化栈
void init(Stack* s) {
    s->top = -1;
}

// 判断栈是否为空
int is_empty(Stack* s) {
    return s->top == -1;
}

// 判断栈是否已满
int is_full(Stack* s) {
    return s->top == MAX_SIZE - 1;
}

// 入栈
void push(Stack* s, int x) {
    if (is_full(s)) {
        printf("Stack is full.\n");
        exit(1);
    }
    s->data[++s->top] = x;
}

// 出栈
int pop(Stack* s) {
    if (is_empty(s)) {
        printf("Stack is empty.\n");
        exit(1);
    }
    return s->data[s->top--];
}

// 获取栈顶元素
int top(Stack* s) {
    if (is_empty(s)) {
        printf("Stack is empty.\n");
        exit(1);
    }
    return s->data[s->top];
}

// 判断一个字符是否为运算符
int is_operator(char ch) {
    return ch == '+' || ch == '-' || ch == '*' || ch == '/';
}

// 计算表达式的值
int evaluate_expression(char* expression) { 
	// 定义运算符优先级数组
    int precedence[] = {0, 1, 1, 2, 2};  // '+', '-', '*', '/'
int i;char ch;int op,operand2,operand1;
    Stack operand_stack;  // 操作数栈
    Stack operator_stack;  // 运算符栈
    init(&operand_stack);
    init(&operator_stack);

  
    // 遍历表达式中的所有字符
    for ( i = 0; expression[i] != '#'; i++) {
       ch  = expression[i];
        // 如果是数字，则将其推入操作数栈中
        if (isdigit(ch)) {
            push(&operand_stack, ch - '0');
        }
        // 如果是左括号，则将其推入运算符栈中
        else if (ch == '(') {
            push(&operator_stack, ch);
        }
        // 如果是右括号，则执行运算直到遇到左括号
        else if (ch == ')') {
            while (top(&operator_stack) != '(') {
               op  = pop(&operator_stack);
               operand2 = pop(&operand_stack);
               operand1 = pop(&operand_stack);
                switch (op) {
                    case '+': push(&operand_stack, operand1 + operand2); break;
                    case '-': push(&operand_stack, operand1 - operand2); break;
                    case '*': push(&operand_stack, operand1 * operand2); break;
                    case '/': push(&operand_stack, operand1 / operand2); break;
                }
            }
            // 弹出左括号
            pop(&operator_stack);
        }
        // 如果是运算符
        else if (is_operator(ch)) {
            // 如果运算符栈为空，则直接if (is_empty(&operator_stack)) {
            push(&operator_stack, ch);
        }
        // 如果当前运算符的优先级高于栈顶运算符的优先级，则将其推入运算符栈中
        else if (precedence[ch - '+'] > precedence[top(&operator_stack) - '+']) {
            push(&operator_stack, ch);
        }
        // 否则执行栈顶运算符的运算，直到当前运算符的优先级大于栈顶运算符的优先级，然后将其推入运算符栈中
        else {
            while (!is_empty(&operator_stack) && precedence[ch - '+'] <= precedence[top(&operator_stack) - '+']) {
                 op = pop(&operator_stack);
                 operand2 = pop(&operand_stack);
                 operand1 = pop(&operand_stack);
                switch (op) {
                    case '+': push(&operand_stack, operand1 + operand2); break;
                    case '-': push(&operand_stack, operand1 - operand2); break;
                    case '*': push(&operand_stack, operand1 * operand2); break;
                    case '/': push(&operand_stack, operand1 / operand2); break;
                }
            }
            push(&operator_stack, ch);
        }
    }

// 执行剩余的运算
while (!is_empty(&operator_stack)) {
     op = pop(&operator_stack);
     operand2 = pop(&operand_stack);
     operand1 = pop(&operand_stack);
    switch (op) {
        case '+': push(&operand_stack, operand1 + operand2); break;
        case '-': push(&operand_stack, operand1 - operand2); break;
        case '*': push(&operand_stack, operand1 * operand2); break;
        case '/': push(&operand_stack, operand1 / operand2); break;
    }
}
// 返回结果
return top(&operand_stack);}

int main() {
char expression[MAX_SIZE];
printf("请输入算数表达式，以#结尾：\n");
scanf("%s", expression);
printf("结果是: %d\n", evaluate_expression(expression));
return 0;
}
