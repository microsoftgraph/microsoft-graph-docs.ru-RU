---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d17ed3461a3d61f5daec52f0c4a1116c9b93f89f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803288"
---
# <a name="omasettingfloatingpoint-resource-type"></a>Тип ресурса omaSettingFloatingPoint

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение плавающей запятой параметра OMA.


Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|Строка|Описание. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|secretReferenceValueId|String|ReferenceId для поисков секрета для расшифровки. Это свойство доступно только для чтения. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|isEncrypted|Boolean|Указывает, зашифровано ли поле значений. Это свойство доступно только для чтения. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|value|Single|Значение.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": 4.2
}
```



