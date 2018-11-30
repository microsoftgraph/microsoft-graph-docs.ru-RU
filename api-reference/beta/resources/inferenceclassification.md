---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
ms.openlocfilehash: c1536ff2b88b1830c2f2a2bc5a7bed519782df4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074699"
---
# <a name="inferenceclassification-resource-type"></a>Тип ресурса inferenceClassification

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. 

Дополнительные сведения см. в статье [Управление сортировкой почты](manage-focused-inbox.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md)| Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.|
|[Список переопределений](../api/inferenceclassification-list-overrides.md) |Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)| Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка| Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|overrides|Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)| Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->