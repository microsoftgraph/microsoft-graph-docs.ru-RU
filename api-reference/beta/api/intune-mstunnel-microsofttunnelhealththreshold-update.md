---
title: Обновление microsoftTunnelHealthThreshold
description: Обновление свойств объекта microsoftTunnelHealthThreshold.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 318ec9d93d995d29c357da02dc756ed34bc04e36
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494054"
---
# <a name="update-microsofttunnelhealththreshold"></a>Обновление microsoftTunnelHealthThreshold

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelHealthThresholds/{microsoftTunnelHealthThresholdId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса подарйте представление JSON для [объекта microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)

В следующей таблице показаны свойства, необходимые при создании [microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Имя метрик|
|healthyThreshold|Int64|Пороговое значение для здоровья|
|unhealthyThreshold|Int64|Порог для неработоспособного|
|defaultHealthyThreshold|Int64|Пороговое значение по умолчанию для того, чтобы быть здоровым|
|defaultUnhealthyThreshold|Int64|Пороговое значение по умолчанию для неработоспособного|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelHealthThresholds/{microsoftTunnelHealthThresholdId}
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "healthyThreshold": 0,
  "unhealthyThreshold": 2,
  "defaultHealthyThreshold": 7,
  "defaultUnhealthyThreshold": 9
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "id": "419c526e-526e-419c-6e52-9c416e529c41",
  "healthyThreshold": 0,
  "unhealthyThreshold": 2,
  "defaultHealthyThreshold": 7,
  "defaultUnhealthyThreshold": 9
}
```



