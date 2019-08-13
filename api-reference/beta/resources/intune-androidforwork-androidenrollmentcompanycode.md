---
title: Тип ресурса Андроиденроллменткомпаникоде
description: Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ccc8cd1c1753c844ac5a71f9248f8189dad1e0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367101"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>Тип ресурса Андроиденроллменткомпаникоде

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|енроллменттокен|String|Маркер регистрации, используемый пользователем для регистрации своего устройства.|
|qrCodeContent|String|Строка, используемая для создания QR-кода маркера.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Созданный QR код для маркера.|

## <a name="relationships"></a>Отношения
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



