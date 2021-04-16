---
title: Создание microsoftTunnelSite
description: Создайте новый объект microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b37330f63c9c0f27ae0d701db59b5795d3f15bf4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864811"
---
# <a name="create-microsofttunnelsite"></a>Создание microsoftTunnelSite

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложения|MicrosoftTunnelGateway.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса устройте представление JSON для объекта microsoftTunnelSite.

В следующей таблице показаны свойства, необходимые при создании microsoftTunnelSite.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id MicrosoftTunnelSite|
|displayName|String|Имя отображения MicrosoftTunnelSite|
|description|String|Описание MicrosoftTunnelSite|
|publicAddress|String|Имя или IP-адрес общественного домена MicrosoftTunnelSite|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




