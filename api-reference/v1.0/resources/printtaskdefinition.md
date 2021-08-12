---
title: тип ресурса printTaskDefinition
description: Представляет задачу, которая может быть вызвана при различных событиях, происходящих в универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c63fb604db54bafd757fe82e2bc21feee005dbda5c91d9c4a7f64b0c1e607dab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149683"
---
# <a name="printtaskdefinition-resource-type"></a>тип ресурса printTaskDefinition

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет абстрактное определение задачи, которая может быть вызвана при различных событиях, происходящих в универсальной печати.

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

Этот ресурс поддерживает:
* [Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/print-list-taskdefinitions.md) | [printTaskDefinition collection](printtaskdefinition.md) | Получите полный список отпечатковTaskDefinitions, созданных в универсальной печати. |
| [Создание](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создайте новый шрифтTaskDefinition. |
| [Обновление](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Обновление печатиTaskDefinition. |
| [Удаление](../api/print-delete-taskdefinition.md) | Нет | Удаление печатиTaskDefinition. |
| [Перечисление задач](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получите список задач, созданных на основе этого определения. Список включает в себя выполнение текущих задач и недавно завершенных задач. |
| [Вывод задачи](../api/printtask-get.md) | [printTask](printtask.md) | Получает задачу, созданную на основе этого определения. |
| [Обновление задачи](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Обновление задачи, созданной на основе этого определения. **Приложения, которые регистрируют триггеры задач, отвечают за обновление состояния задачи по завершению обработки, если соответствующий printJob не был перенаправлен на другой принтер.** Невыполнение отчетов о завершении приведет к блокировке связанного задания печати от печати и в конечном итоге к их удаляемой работе. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор printTaskDefinition. Только для чтения.|
|displayName|String|Имя печатиTaskDefinition.|
|createdBy|[appIdentity](appidentity.md)|Приложение, создав печатьTaskDefinition. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|tasks|[printTask](printtask.md) collection|Список задач, созданных на основе этого определения. Список включает в себя выполнение текущих задач и недавно завершенных задач. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.appIdentity"
  }
}
```

