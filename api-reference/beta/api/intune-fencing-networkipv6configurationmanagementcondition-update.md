---
title: Обновление networkIPv6ConfigurationManagementCondition
description: Обновление свойств объекта networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55f01259d3301859cb0e4af948ca25f596053218
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257756"
---
# <a name="update-networkipv6configurationmanagementcondition"></a>Обновление networkIPv6ConfigurationManagementCondition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)

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
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)

В следующей таблице показаны свойства, необходимые при создании [networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для состояния управления. Созданное в системе значение, назначенное при его создания. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Строка|Уникальное имя для состояния управления. Используется в выражениях условий управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Администратор определил имя условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Строка|Администратор определил описание условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Сгенерированная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag состояния управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[коллекция devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|Применимые платформы для этого условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ipV6Prefix|String|Подсеть IPv6, к которая должна быть подключена. например, 2001:db8::/32|
|ipV6Gateway|String|Адрес шлюза IPv6. например, 2001:db8::1|
|ipV6DNSServerList|Коллекция String|DNS-серверы IPv6, настроенные для адаптеров.|
|dnsSuffixList|Коллекция String|Допустимые Суффиксы DNS для текущей сети. например, seattle.contoso.com|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




