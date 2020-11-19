---
title: Тип ресурса windows10XWifiConfiguration
description: Профиль конфигурации Windows X Вификсмл
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1353597c05d1f661474f563b6dee3c07fe408f77
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302008"
---
# <a name="windows10xwificonfiguration-resource-type"></a>Тип ресурса windows10XWifiConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации Windows X Вификсмл


Наследуется от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10XWifiConfigurations](../api/intune-rapolicy-windows10xwificonfiguration-list.md)|Коллекция [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Список свойств и связей объектов [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|
|[Получение windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-get.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Чтение свойств и связей объекта [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|
|[Создание windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-create.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Создание нового объекта [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|
|[Удаление windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-delete.md)|Нет|Удаляет объект [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md).|
|[Обновление windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-update.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Обновление свойств объекта [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор профиля унаследован от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|version|Int32|Версия профиля, унаследованного от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|Отображаемое имя профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|String|Описание профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|креатиондатетиме|DateTimeOffset|Создан профиль DateTime, наследуемый от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение профиля DateTime унаследовано от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|Коллекция строк|Теги областей унаследованы от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|аусентикатионцертификатеид|Guid|Идентификатор сертификата проверки подлинности|
|кустомксмлфиленаме|String|Имя настраиваемого XML-файла.|
|customXml|Binary|Настраиваемые XML-команды, которые настраивают VPN-подключение. (Кодирование байтов в кодировке UTF8)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XWifiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "authenticationCertificateId": "Guid",
  "customXmlFileName": "String",
  "customXml": "binary"
}
```




