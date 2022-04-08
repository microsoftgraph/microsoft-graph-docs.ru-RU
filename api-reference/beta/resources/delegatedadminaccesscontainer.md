---
title: Тип ресурса delegatedAdminAccessContainer
description: Контейнер доступа администратора, с помощью которого роли каталога назначаются с помощью назначения доступа.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 330cbb49f1ad78f327b3d00c9b04b16004de2969
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704333"
---
# <a name="delegatedadminaccesscontainer-resource-type"></a>Тип ресурса delegatedAdminAccessContainer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер доступа администратора, с помощью которого роли каталога назначаются с помощью назначения доступа.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessContainerId|String|Идентификатор контейнера доступа (например, группы безопасности). Для контейнеров доступа securityGroup это должен быть допустимый идентификатор группы безопасности Azure AD в клиенте партнера Майкрософт.|
|accessContainerType|delegatedAdminAccessContainerType|Тип контейнера доступа (например, группа безопасности), который будет назначен одной или нескольким ролям через делегированное отношение администратора. Возможные значения: `securityGroup`, `unknownFutureValue`.|

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

