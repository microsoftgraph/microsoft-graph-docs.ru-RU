---
title: Тип ресурса deviceInstallState
description: Содержит свойства состояния установки для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51024339ac6d4bae38e6e6a54dc23cba7bb6b94e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806700"
---
# <a name="deviceinstallstate-resource-type"></a>Тип ресурса deviceInstallState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства состояния установки для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceInstallStates](../api/intune-books-deviceinstallstate-list.md)|Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Получение объекта deviceInstallState](../api/intune-books-deviceinstallstate-get.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Чтение свойств и связей объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Создание объекта deviceInstallState](../api/intune-books-deviceinstallstate-create.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Удаление объекта deviceInstallState](../api/intune-books-deviceinstallstate-delete.md)|Нет|Удаляет объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Обновление объекта deviceInstallState](../api/intune-books-deviceinstallstate-update.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Обновление свойств объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|deviceName|String|Имя устройства.|
|deviceId|String|Идентификатор устройства.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации.|
|installState|[installState](../resources/intune-books-installstate.md)|Состояние установки электронной книги. Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|errorCode|String|Код ошибки для сбоев при установке.|
|osVersion|String|Версия ОС.|
|osDescription|String|Описание ОС.|
|userName|String|Имя пользователя устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



