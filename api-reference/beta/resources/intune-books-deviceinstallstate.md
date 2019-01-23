---
title: Тип ресурса deviceInstallState
description: Содержит свойства состояния установки для устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c90b3e8e0693a28781a45f77cd00661528648439
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410723"
---
# <a name="deviceinstallstate-resource-type"></a>Тип ресурса deviceInstallState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Ключ объекта.|
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




