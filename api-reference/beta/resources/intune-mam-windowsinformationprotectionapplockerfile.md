---
title: Тип ресурса windowsInformationProtectionAppLockerFile
description: Файл AppLocker для Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fa50f676ed559477218286740a1a2f02f7d17afc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527851"
---
# <a name="windowsinformationprotectionapplockerfile-resource-type"></a>Тип ресурса windowsInformationProtectionAppLockerFile

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Файл AppLocker для Windows Information Protection

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-list.md)|Коллекция [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Получение объекта windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md);|Чтение свойств и связей объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Создание объекта windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-create.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md);|Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Удаление объекта windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-delete.md)|Нет|Удаляет объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Обновление объекта windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-update.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Понятное имя|
|fileHash|String|Хэш SHA256 для файла|
|file|Binary|Файл в виде массива байтов|
|id|String|Ключ объекта.|
|version|Строка|Версия объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "String",
  "fileHash": "String",
  "file": "binary",
  "id": "String (identifier)",
  "version": "String"
}
```



