---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
ms.openlocfilehash: c45abb14669c3cf67571748a9da7d62bed037ff6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325825"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>Тип ресурса windowsInformationProtectionDataRecoveryCertificate

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сертификат восстановления данных Windows Information Protection
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|subjectName|String|Имя субъекта для сертификата восстановления данных|
|описание|String|Описание сертификата восстановления данных|
|expirationDateTime|DateTimeOffset|Дата и время окончания срока действия для сертификата восстановления данных|
|certificate|Двоичный|Сертификат восстановления данных|

## <a name="relationships"></a>Связи
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





