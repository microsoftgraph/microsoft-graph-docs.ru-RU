---
title: тип ресурса deviceManagementSettingEnrollmentTypeConstraint
description: Ограничение, которое обеспечивает соблюдение типов регистрации, примененных к параметру
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbc0cc62fefad3ddd6411a964edceafc486ab9f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134915"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a>тип ресурса deviceManagementSettingEnrollmentTypeConstraint

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, которое обеспечивает соблюдение типов регистрации, примененных к параметру


Наследует [от deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enrollmentTypes|Коллекция объектов string|Список типов регистрации|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```



