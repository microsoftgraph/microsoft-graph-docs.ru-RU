---
title: Тип ресурса Андроиденроллменткомпаникоде
description: Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd37bcb9dba4e4fc6ce54e686a6a889ce73448d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495174"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>Тип ресурса Андроиденроллменткомпаникоде

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|енроллменттокен|String|Маркер регистрации, используемый пользователем для регистрации своего устройства.|
|qrCodeContent|String|Строка, используемая для создания QR-кода маркера.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Созданный QR код для маркера.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



