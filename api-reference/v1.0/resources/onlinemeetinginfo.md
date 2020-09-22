---
title: Тип ресурса Онлинемитингинфо
description: Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6085c40e3d45e27e6c60ec516f781f40621f34c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079006"
---
# <a name="onlinemeetinginfo-resource-type"></a>Тип ресурса Онлинемитингинфо

Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|конференцеид|Строка| Идентификатор конференции.|
|жоинурл|Строка| Внешняя ссылка, которая запускает собрание по сети. Это URL-адрес, который клиенты будут запускать в браузере и перенаправит пользователя для присоединения к собранию.|
|phones|Коллекция [phone](phone.md)| Все номера телефонов, связанные с этой Конференции.|
|куиккдиал|Строка| Предварительно отформатированный куиккдиал для этого вызова.|
|толлфринумберс|Коллекция String| Бесплатных бесплатных номеров, которые можно использовать для присоединения к Конференции.|
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
}-->

