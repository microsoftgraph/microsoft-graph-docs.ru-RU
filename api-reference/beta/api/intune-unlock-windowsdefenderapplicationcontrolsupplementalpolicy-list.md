---
title: Список ВиндовсдефендераппликатионконтролсупплементалполиЦиес
description: Список свойств и связей объектов Виндовсдефендераппликатионконтролсупплементалполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51a5bd30fa44b56cc8b0e69eefcd4ecf18d14d1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457547"
---
# <a name="list-windowsdefenderapplicationcontrolsupplementalpolicies"></a>Список ВиндовсдефендераппликатионконтролсупплементалполиЦиес

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
      "id": "83d0c39e-c39e-83d0-9ec3-d0839ec3d083",
      "displayName": "Display Name value",
      "description": "Description value",
      "content": "Y29udGVudA==",
      "contentFileName": "Content File Name value",
      "version": "Version value",
      "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```





