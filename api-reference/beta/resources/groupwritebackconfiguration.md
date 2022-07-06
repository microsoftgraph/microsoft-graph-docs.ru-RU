---
title: Тип ресурса groupWritebackConfiguration
description: Указывает, включена ли обратная запись облачных групп в локальную службу Active Directory и тип целевой группы для локальной группы.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 45b14ce9fc0e687c5fbc2cd20fc7b63509d54a0f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645387"
---
# <a name="groupwritebackconfiguration-resource-type"></a>Тип ресурса groupWritebackConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, включена ли обратная запись облачных групп в локальную службу Active Directory и тип целевой группы для локальной группы.

 По умолчанию все группы Azure AD безопасности не поддерживают обратную запись. Для групп Microsoft 365 параметры по умолчанию, определенные свойствами этого ресурса, `NewUnifiedgroupWritebackDefault` могут быть перезаписаны объектом [параметра каталога](directorysetting.md).

Наследуется [от writebackConfiguration](../resources/writebackconfiguration.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена ли обратная запись облачных групп в локальную службу Active Directory. Допускается значение null. Значение по умолчанию — `true` для групп Microsoft 365 и `false` групп безопасности. Наследуется [от writebackConfiguration](../resources/writebackconfiguration.md).|
|onPremisesGroupType|String|Указывает тип целевой локальной группы, в который будет записан облачный объект. Допускается значение null. Допустимые значения: `universalDistributionGroup`, `universalSecurityGroup`, `universalMailEnabledSecurityGroup`.<ol><li>Если облачная группа является единой группой (Microsoft 365), это свойство может иметь одно из следующих значений: `universalDistributionGroup`, `universalSecurityGroup`, `universalMailEnabledSecurityGroup`. </li><li>Azure AD группы безопасности можно записать обратно как `universalSecurityGroup`. </li><li>Если **параметр isEnabled** или group `NewUnifiedGroupWritebackDefault` [имеет](directorysetting.md) значение `true` , но это свойство не настроено явным образом: <ul><li>Группы Microsoft 365 будут записаны по `universalDistributionGroup` умолчанию</li></ul><ul><li>Группы безопасности будут записаны как по `universalSecurityGroup` умолчанию</li></ul>|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupWritebackConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupWritebackConfiguration",
  "isEnabled": "Boolean",
  "onPremisesGroupType": "String"
}
```

