---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88a3b9054e9e274b1acdd4109c6d1b267784cc26
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733712"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет объект пользователя Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление пользователей](../api/intune-mam-user-list.md)|Коллекция объектов [user](../resources/intune-mam-user.md)|Список свойств и связей объектов [user](../resources/intune-mam-user.md).|
|[Получение пользователя](../api/intune-mam-user-get.md)|[user](../resources/intune-mam-user.md)|Чтение свойств и связей объекта [user](../resources/intune-mam-user.md).|
|[Создание пользователя](../api/intune-mam-user-create.md)|[user](../resources/intune-mam-user.md)|Создание объекта [user](../resources/intune-mam-user.md).|
|[Удаление пользователя](../api/intune-mam-user-delete.md)|Нет|Удаляет объект [user](../resources/intune-mam-user.md).|
|[Обновление пользователя](../api/intune-mam-user-update.md)|[user](../resources/intune-mam-user.md)|Обновление свойств объекта [user](../resources/intune-mam-user.md).|
|[Функция getManagedAppDiagnosticStatuses](../api/intune-mam-user-getmanagedappdiagnosticstatuses.md)|Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)|Получает состояние диагностической проверки определенного пользователя.|
|[Функция getManagedAppPolicies](../api/intune-mam-user-getmanagedapppolicies.md)|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Получает ограничения приложений для определенного пользователя.|
|[Действие wipeManagedAppRegistrationsByDeviceTag](../api/intune-mam-user-wipemanagedappregistrationsbydevicetag.md)|Нет|Стирает данные о регистрации приложений с указанным тегом приложения.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```





