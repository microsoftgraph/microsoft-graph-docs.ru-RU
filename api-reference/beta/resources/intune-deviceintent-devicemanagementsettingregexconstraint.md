---
title: тип ресурса deviceManagementSettingRegexConstraint
description: Ограничение, принудительное выполнение параметров, совпадающих с заданным шаблоном RegEx
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e548037fffc5839a097a793ec8ab6c833c344cee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115361"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a>тип ресурса deviceManagementSettingRegexConstraint

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, принудительное выполнение параметров, совпадающих с заданным шаблоном RegEx


Наследует [от deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|regex|String|Шаблон RegEx, который соответствует|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```



