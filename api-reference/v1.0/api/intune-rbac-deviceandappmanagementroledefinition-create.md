---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0875812bf8ee125d34c396caae2f0078f1e6faf1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960253"
---
# <a name="create-deviceandappmanagementroledefinition"></a>Создание deviceAndAppManagementRoleDefinition

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementRBAC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.

В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически. Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|displayName|String|Отображаемое имя определения роли. Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|description|String|Описание определения роли. Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|rolePermissions|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission. Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|isBuiltIn|Boolean|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False. Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|



## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



