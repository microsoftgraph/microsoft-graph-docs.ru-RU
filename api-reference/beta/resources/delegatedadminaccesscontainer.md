---
title: делегирован тип ресурса DelegatedAdminAccessContainer
description: Контейнер доступа администратора, через который роли каталога назначены с помощью назначения доступа.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0f129195430f51ca3102f38db5730eb36ea4d7a8
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589995"
---
# <a name="delegatedadminaccesscontainer-resource-type"></a>делегирован тип ресурса DelegatedAdminAccessContainer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер доступа администратора, через который роли каталога назначены с помощью назначения доступа.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessContainerId|Строка|Идентификатор контейнера доступа (например, группы безопасности). Для контейнеров доступа "SecurityGroup" это должен быть действительный удостоверение группы безопасности Azure AD в клиенте партнера Майкрософт.|
|accessContainerType|delegatedAdminAccessContainerType|Тип контейнера доступа (например, группы безопасности), который будет назначен одной или несколько ролей через делегированную связь администратора. Возможные значения: `securityGroup`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessContainer",
  "accessContainerId": "String",
  "accessContainerType": "String"
}
```

