---
title: тип ресурса windows10XTrustedRootCertificate
description: Windows X Доверенный профиль конфигурации корневого сертификата
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44bc361d35c024e8e4204764831d3c8195ef4954
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788165"
---
# <a name="windows10xtrustedrootcertificate-resource-type"></a>тип ресурса windows10XTrustedRootCertificate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows X Доверенный профиль конфигурации корневого сертификата


Наследует [от deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10XTrustedRootCertificates](../api/intune-rapolicy-windows10xtrustedrootcertificate-list.md)|[коллекция windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Список свойств и связей [объектов Windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|
|[Get windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-get.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Чтение свойств и связей [объекта Windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|
|[Создание windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-create.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Создайте [новый объект Windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|
|[Удаление windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-delete.md)|Нет|Удаляет [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).|
|[Обновление windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-update.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Обновление свойств объекта [windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|version|Int32|Версия профиля, унаследованной от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|Строка|Имя отображения профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|Строка|Описание профиля, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|creationDateTime|DateTimeOffset|Профиль DateTime был создан по наследству от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|Последний раз был изменен профиль DateTime, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|Коллекция String|Теги области, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|trustedRootCertificate|В двоичном формате|Надежный корневой сертификат|
|certFileName|Строка|Имя файла для отображения в пользовательском интерфейсе.|
|destinationStore|[certificateDestinationStore](../resources/intune-shared-certificatedestinationstore.md)|Расположение магазина назначения для доверенного корневого сертификата. Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Список назначений для профиля конфигурации устройства. Унаследовано от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XTrustedRootCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "destinationStore": "String"
}
```



