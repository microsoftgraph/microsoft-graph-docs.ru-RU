---
title: Обновление windowsDefenderApplicationControlSupplementalPolicy
description: Обновление свойств объекта WindowsDefenderApplicationControlSupplementalPolicy.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a53b4f9a9a1460cf5c58d0fecf62eb55b1e58cd2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047886"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a>Обновление windowsDefenderApplicationControlSupplementalPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)

В следующей таблице показаны свойства, необходимые при создании [windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ для дополнительной политики WindowsDefenderApplicationControl.|
|displayName|String|Отображение имени дополнительной политики WindowsDefenderApplicationControl.|
|description|String|Описание дополнительной политики WindowsDefenderApplicationControl.|
|содержимое|В двоичном формате|Контент дополнительной политики WindowsDefenderApplicationControl в формате byte array.|
|contentFileName|String|Имя файла дополнительного контента политики WindowsDefenderApplicationControl.|
|version|String|Версия дополнительной политики WindowsDefenderApplicationControl.|
|creationDateTime|DateTimeOffset|Дата и время отправки дополнительной политики WindowsDefenderApplicationControl.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения политики дополнительных приложений WindowsDefenderApplicationControl.|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого объекта дополнительной политики WindowsDefenderApplicationControl.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 517

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
```



