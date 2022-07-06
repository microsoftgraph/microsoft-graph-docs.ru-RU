---
title: Тип ресурса teamsAppSettings
description: Представляет параметры приложения Teams
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a36f6657dc8231450514eb6c60d7d729c0e0818
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645744"
---
# <a name="teamsappsettings-resource-type"></a>Тип ресурса teamsAppSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры на уровне клиента для всех [приложений Teams](teamsapp.md) в клиенте.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение teamsAppSettings](../api/teamsappsettings-get.md)|[teamsAppSettings](../resources/teamsappsettings.md)|Получение параметров на уровне клиента для всех приложений Teams в клиенте.|
|[Обновление teamsAppSettings](../api/teamsappsettings-update.md)|[teamsAppSettings](../resources/teamsappsettings.md)|Обновите параметры на уровне клиента для всех приложений Teams в клиенте.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isChatResourceSpecificConsentEnabled|Boolean|Указывает, включено ли для клиента согласие на чаты и собрания для конкретного ресурса. Если значение равно true, приложения Teams, которые разрешены в клиенте и требуют разрешений для конкретных ресурсов, можно устанавливать в чатах и собраниях. Если задано значение false, установка любого приложения Teams, для которого требуются разрешения конкретного ресурса в чате или на собрании, будет заблокирована.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppSettings",
  "id": "String (identifier)",
  "isChatResourceSpecificConsentEnabled": "Boolean"
}
```

## <a name="see-also"></a>См. также

- [Согласие для определенных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)