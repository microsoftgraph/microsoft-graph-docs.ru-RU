---
title: Создание пользователя
description: Создание объекта user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5f176313c00787cf29de232589dc2029408e927
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787920"
---
# <a name="create-user"></a>Создание пользователя

Пространство имен: microsoft.graph

> **Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [user](../resources/intune-shared-user.md).

## <a name="prerequisites"></a>Предварительные условия

Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).  Необходимое разрешение зависит от контекста.

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **Устранение неполадок** | DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application||
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All|
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All|
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; **Устранение неполадок** | DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a>Заголовки запроса

|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса

В теле запроса добавьте представление объекта user в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор пользователя.|
|**На посадке**||
|deviceEnrollmentLimit|Int32|Максимальное количество устройств, которые разрешено зарегистрировать пользователю. Допустимые значения: 5 или 1000.|

Поддержка свойств тела запроса зависит от контекста.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. Свойства, возвращенные при фактическом вызове, различаются в зависимости от контекста.

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









