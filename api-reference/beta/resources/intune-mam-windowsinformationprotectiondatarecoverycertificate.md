---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52377b6b94357edfdd5c3c9945f3aefe30695968
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030039"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>Тип ресурса windowsInformationProtectionDataRecoveryCertificate

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сертификат восстановления данных Windows Information Protection

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|subjectName|String|Имя субъекта для сертификата восстановления данных|
|description|String|Описание сертификата восстановления данных|
|expirationDateTime|DateTimeOffset|Дата и время окончания срока действия для сертификата восстановления данных|
|certificate|Двоичный|Сертификат восстановления данных|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```






