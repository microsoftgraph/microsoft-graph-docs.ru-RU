---
title: Тип ресурса userInstallStateSummary
description: Содержит свойства сводки по состоянию установки для пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8372687b174c5c7e1997227df48bac82afecffa4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694020"
---
# <a name="userinstallstatesummary-resource-type"></a>Тип ресурса userInstallStateSummary

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сводки по состоянию установки для пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов userInstallStateSummary](../api/intune-books-userinstallstatesummary-list.md)|Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Получение объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Создание объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-create.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Удаление объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-delete.md)|Нет|Удаляет объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|
|[Обновление объекта userInstallStateSummary](../api/intune-books-userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Обновление свойств объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
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





