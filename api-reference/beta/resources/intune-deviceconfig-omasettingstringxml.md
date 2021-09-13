---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c269f3c2bf5bb59a813813e4a5f26f53e595c594
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057469"
---
# <a name="omasettingstringxml-resource-type"></a>Тип ресурса omaSettingStringXml

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение строки параметра OMA в формате XML.


Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Описание. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|String|OMA. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|secretReferenceValueId|String|ReferenceId для поисков секрета для расшифровки. Это свойство доступно только для чтения. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|isEncrypted|Boolean|Указывает, зашифровано ли поле значений. Это свойство доступно только для чтения. Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|String|Имя файла, связанное со свойством Value (XML).|
|value|Двоичный|Значение (массив байтов в кодировке UTF8).|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "binary"
}
```



