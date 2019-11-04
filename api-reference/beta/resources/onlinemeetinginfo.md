---
title: Тип ресурса Онлинемитингинфо
description: Сведения для участников, присоединяющихся к собранию в Интернете.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ed8543be8b1d22c797d0033dcd0d41ba6308888
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939392"
---
# <a name="onlinemeetinginfo-resource-type"></a>Тип ресурса Онлинемитингинфо

Сведения для участников, присоединяющихся к собранию в Интернете.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|конференцеид|Строка| Идентификатор конференции.|
|жоинурл|Строка| Внешняя ссылка, которая запускает собрание по сети. Это URL-адрес, который клиенты будут запускать в браузере и перенаправит пользователя для присоединения к собранию.|
|phones|Коллекция [phone](phone.md)| Все номера телефонов, связанные с этой Конференции.|
|куиккдиал|Строка| Предварительно отформатированный куиккдиал для этого вызова.|
|толлфринумберс|Коллекция строк| Бесплатных бесплатных номеров, которые можно использовать для присоединения к Конференции.|
|толлнумбер|Строка| Платный номер, который можно использовать для присоединения к Конференции.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}-->

```json
{
  "conferenceId": "String",
  "joinUrl": "String",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "quickDial": "String",
  "tollFreeNumbers": ["String"],
  "tollNumber": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->s
