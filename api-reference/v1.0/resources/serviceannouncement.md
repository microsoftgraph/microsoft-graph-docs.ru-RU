---
title: тип ресурса serviceAnnouncement
description: Контейнер верхнего уровня для ресурсов связи службы
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 5af86f432bb26495111feff7a33adeca2d54f372
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019148"
---
# <a name="serviceannouncement-resource-type"></a>тип ресурса serviceAnnouncement

Пространство имен: microsoft.graph

Контейнер верхнего уровня для ресурсов связи службы.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список healthOverviews](../api/serviceannouncement-list-healthoverviews.md)|[коллекция serviceHealth](../resources/servicehealth.md)|Получите ресурсы serviceHealth из свойства навигации healthOverviews.|
|[Проблемы со списком](../api/serviceannouncement-list-issues.md)|[коллекция serviceHealthIssue](../resources/servicehealthissue.md)|Получите ресурсы serviceHealthIssue из свойства навигации проблем.|
|[Список сообщений](../api/serviceannouncement-list-messages.md)|[коллекция serviceUpdateMessage](../resources/serviceupdatemessage.md)|Получите ресурсы serviceUpdateMessage из свойства навигации сообщений.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Свойство|Тип|Описание|
|-|-|-|
|messages|[Collection(serviceUpdateMessage)](serviceupdatemessage.md)|Коллекция сообщений службы для клиента. Это свойство содержит свойство навигации, оно является недействительным и читаемым.|
|healthOverviews|[Collection(serviceHealth)](servicehealth.md)|Коллекция сведений о состоянии здоровья служб для клиента. Это свойство содержит свойство навигации, оно является недействительным и читаемым.|
|проблемы|[Collection(serviceHealthIssue)](servicehealthissue.md)|Набор проблем с обслуживанием для клиента. Это свойство содержит свойство навигации, оно является недействительным и читаемым.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncement"
}
```
