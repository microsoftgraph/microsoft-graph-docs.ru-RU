---
title: Обновление networkIPv4ConfigurationManagementCondition
description: Обновление свойств объекта networkIPv4ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9e776dfaef1a1b7c0fe2c005bf7847c5ab8e0e2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157544"
---
# <a name="update-networkipv4configurationmanagementcondition"></a>Обновление networkIPv4ConfigurationManagementCondition

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [networkIPv4ConfigurationManagementCondition.](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта networkIPv4ConfigurationManagementCondition.](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)

В следующей таблице показаны свойства, необходимые при создании [networkIPv4ConfigurationManagementCondition.](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для состояния управления. Созданное в системе значение, назначенное при его создания. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Строка|Уникальное имя для состояния управления. Используется в выражениях условий управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Строка|Администратор определил имя условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Строка|Администратор определил описание условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Сгенерированная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag состояния управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[коллекция devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Применимые платформы для этого условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ipV4Prefix|Строка|Подсеть IPv4, к которая должна быть подключена. например, 10.0.0.0/8|
|ipV4Gateway|Строка|Адрес шлюза IPv4. например, 10.0.0.0|
|ipV4DHCPServer|Строка|Адрес IPv4 сервера DHCP для адаптер.|
|ipV4DNSServerList|Коллекция String|Серверы DNS IPv4, настроенные для адаптеров.|
|dnsSuffixList|Коллекция String|Допустимые Суффиксы DNS для текущей сети. например, seattle.contoso.com|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
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
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




