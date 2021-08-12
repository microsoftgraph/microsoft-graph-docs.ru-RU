---
title: тип ресурса serviceUpdateMessageViewpoint
description: Представляет данные точек представления пользователей для службыUpdateMessage".
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 2d35d04c243469eb72cb0ad85cb269d7de32a4b0642dfb3489963f6f2a294813
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195609"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>тип ресурса serviceUpdateMessageViewpoint

Пространство имен: microsoft.graph

Представляет данные точек представления пользователей для [службыUpdateMessage.](../resources/serviceupdatemessage.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isArchived|Boolean|Указывает, архивировать ли сообщение пользователь.|
|isFavorited|Логический|Указывает, отметил ли пользователь сообщение как избранное.|
|isRead|Boolean|Указывает, читал ли пользователь сообщение.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessageViewpoint",
  "isRead": "Boolean",
  "isArchived": "Boolean",
  "isFavorited": "Boolean"
}
```