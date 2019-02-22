---
title: Обновление Иосвппаппассигнедусерлиценсе
description: Обновление свойств объекта Иосвппаппассигнедусерлиценсе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa78f8d523c0c09e64f0d4c198a631789425a821
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152908"
---
# <a name="update-iosvppappassigneduserlicense"></a>Обновление Иосвппаппассигнедусерлиценсе

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [Иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|Усеремаиладдресс|String|Адрес электронной почты пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|Идентификатор пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|Имя пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|Строка|Имя участника-пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




