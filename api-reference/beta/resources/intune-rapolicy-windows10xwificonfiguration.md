---
title: тип ресурса windows10XWifiConfiguration
description: Windows X профиль конфигурации WifiXml
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e73fc29134616b421c2a344e62d93f6188dc794
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030160"
---
# <a name="windows10xwificonfiguration-resource-type"></a>тип ресурса windows10XWifiConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows X профиль конфигурации WifiXml


Наследует [от deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10XWifiConfigurations](../api/intune-rapolicy-windows10xwificonfiguration-list.md)|[коллекция windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Список свойств и связей [объектов Windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|
|[Получить windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-get.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Чтение свойств и связей [объекта Windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|
|[Создание windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-create.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Создайте [новый объект Windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|
|[Удаление windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-delete.md)|Нет|Удаляет [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md).|
|[Обновление windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-update.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Обновление свойств объекта [Windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|version|Int32|Версия профиля, унаследованной от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|Имя отображения профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|Строка|Описание профиля, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|creationDateTime|DateTimeOffset|Профиль DateTime был создан по наследству от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|Последний раз был изменен профиль DateTime, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|Коллекция строк|Теги области, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|authenticationCertificateId|Guid|ID к сертификату проверки подлинности|
|customXmlFileName|Строка|Пользовательское имя файла Xml.|
|customXml|В двоичном формате|Настраиваемые XML-команды, настраиваемые vpn-подключением. (кодификат byte UTF8)|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Список назначений для профиля конфигурации устройства. Унаследовано от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

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



