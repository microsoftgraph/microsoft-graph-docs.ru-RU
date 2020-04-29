---
title: Тип ресурса Онлинемитингинфо
description: Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 063f2f43f98d9f2d75822f712c4e17755bc290f7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229453"
---
# <a name="onlinemeetinginfo-resource-type"></a>Тип ресурса Онлинемитингинфо

Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|конференцеид|String| Идентификатор конференции.|
|жоинурл|String| Внешняя ссылка, которая запускает собрание по сети. Это URL-адрес, который клиенты будут запускать в браузере и перенаправит пользователя для присоединения к собранию.|
|phones|Коллекция [phone](phone.md)| Все номера телефонов, связанные с этой Конференции.|
|куиккдиал|String| Предварительно отформатированный куиккдиал для этого вызова.|
|толлфринумберс|Коллекция объектов string| Бесплатных бесплатных номеров, которые можно использовать для присоединения к Конференции.|
|толлнумбер|String| Платный номер, который можно использовать для присоединения к Конференции.|

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
}-->
