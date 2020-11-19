---
title: Тип ресурса windows10XVpnConfiguration
description: Профиль конфигурации виртуальной частной сети Windows X
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cce0be552b22e52476ee704606bd43e7c20f4ec7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302298"
---
# <a name="windows10xvpnconfiguration-resource-type"></a>Тип ресурса windows10XVpnConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации виртуальной частной сети Windows X


Наследуется от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10XVpnConfigurations](../api/intune-rapolicy-windows10xvpnconfiguration-list.md)|Коллекция [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Список свойств и связей объектов [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|
|[Получение windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-get.md)|[windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Чтение свойств и связей объекта [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|
|[Создание windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-create.md)|[windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Создание нового объекта [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|
|[Удаление windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-delete.md)|Нет|Удаляет объект [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md).|
|[Обновление windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-update.md)|[windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Обновление свойств объекта [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|

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
  "@odata.type": "microsoft.graph.windows10XVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
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




