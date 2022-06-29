---
title: Тип ресурса groupWritebackConfiguration
description: Указывает, включена ли обратная запись облачных групп в локальную службу Active Directory и тип целевой группы для локальной группы.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1b546da83c3f53ad1b8126e2967e224e9569cbf5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439694"
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
|onPremisesGroupType|String|Указывает тип целевой локальной группы, в который будет записан облачный объект. Допускается значение null. Допустимые значения: `universalDistributionGroup`, `universalSecurityGroup`, `universalMailEnabledSecurityGroup`. <br>+ Если облачная группа является единой группой (Microsoft 365), это свойство может иметь одно из следующих значений: `universalDistributionGroup`, `universalSecurityGroup`, `universalMailEnabledSecurityGroup`. <br> + Azure AD группы безопасности можно записать обратно как `universalSecurityGroup`. <br> + Если **isEnabled** или параметр `NewUnifiedGroupWritebackDefault` [группы](directorysetting.md) задан `true` , но это свойство не настроено явным образом: <br> &nbsp;&nbsp; + Группы Microsoft 365 будут записаны по `universalDistributionGroup` умолчанию <br> &nbsp;&nbsp; + Группы безопасности будут записаны как по `universalSecurityGroup` умолчанию|

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

