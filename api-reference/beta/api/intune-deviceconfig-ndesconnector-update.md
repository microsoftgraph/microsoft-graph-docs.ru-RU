---
title: Обновление ndesConnector
description: Обновление свойств объекта ndesConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26b4903ce436724c974905b7ecfaabfeb195e49f2771a3bdc16b8476341e9d3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164939"
---
# <a name="update-ndesconnector"></a>Обновление ndesConnector

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)

В следующей таблице показаны свойства, необходимые при создании [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ соединиттеля NDES.|
|lastConnectionDateTime|DateTimeOffset|Последнее время подключения для соединитетеля Ndes|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Состояние соединитетеля Ndes. Возможные значения: `none`, `active`, `inactive`.|
|displayName|Строка|Дружеское имя соединиттеля Ndes.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```




