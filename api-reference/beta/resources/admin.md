---
title: Тип ресурса admin
description: Сущность, которая выступает в качестве контейнера для функций администратора.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ef9b235a175b3304b9354beddc67f59eb3994cf1
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653499"
---
# <a name="admin-resource-type"></a>Тип ресурса admin

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сущность, которая выступает в качестве контейнера для функций администратора.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
| serviceAnnouncement | [serviceAnnouncement](serviceannouncement.md) | Контейнер для ресурсов связи со службами. Только для чтения. |
| sharepoint |[microsoft.graph.tenantAdmin.sharepoint](../resources/tenantadmin-sharepoint.md)|Контейнер для административных ресурсов для управления параметрами на уровне клиента для SharePoint и OneDrive.|
| windows |[microsoft.graph.windowsUpdates.windows](../resources/windowsupdates-windows.md)|Контейнер для всех функций клиентский компонент Центра обновления Windows развертывания для бизнеса. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.admin",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.admin"
}
```

