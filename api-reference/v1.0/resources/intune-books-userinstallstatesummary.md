---
title: Тип ресурса userInstallStateSummary
description: Содержит свойства сводки по состоянию установки для пользователя.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 407dfca3235111ab58ee9327b1a7cee09f5a568b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360435"
---
# <a name="userinstallstatesummary-resource-type"></a>Тип ресурса userInstallStateSummary

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сводки по состоянию установки для пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов userInstallStateSummary](../api/intune-books-userinstallstatesummary-list.md)|Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Получение объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md);|Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Создание объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-create.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md);|Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Удаление объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-delete.md)|Нет|Удаляет объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Обновление объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Обновление свойств объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|userName|String|Имя пользователя.|
|installedDeviceCount|Int32|Количество установленных устройств.|
|failedDeviceCount|Int32|Количество устройств со сбоями.|
|notInstalledDeviceCount|Int32|Количество не установленных устройств.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceStates|Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Состояние установки электронной книги.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```




