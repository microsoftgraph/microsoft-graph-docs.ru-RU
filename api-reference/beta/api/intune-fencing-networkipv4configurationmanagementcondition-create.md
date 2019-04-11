---
title: Создание networkIPv4ConfigurationManagementCondition
description: Создание нового объекта networkIPv4ConfigurationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6459876d0ee318ed3d855a5ff03cb43599773ca3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774549"
---
# <a name="create-networkipv4configurationmanagementcondition"></a>Создание networkIPv4ConfigurationManagementCondition

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта networkIPv4ConfigurationManagementCondition в формате JSON.

В следующей таблице приведены свойства, необходимые при создании networkIPv4ConfigurationManagementCondition.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для условия управления. Созданное системой значение, назначаемое при создании. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Уникальное имя условия управления. Используется в выражениях условия управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Имя условия управления, определенное администратором. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|description|String|Описание условия управления, заданное администратором. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Созданная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|eTag|String|Тег ETag условия управления. Обновленная сторона службы. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|Аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого условия управления. НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.|
|ipV4Prefix|String|Подсеть IPv4, к которой необходимо подключиться. Например, 10.0.0.0/8|
|ipV4Gateway|String|IPv4-адрес шлюза. Например, 10.0.0.0|
|ipV4DHCPServer|String|IPv4-адрес DHCP-сервера для адаптера.|
|ipV4DNSServerList|Коллекция String|DNS-серверы IPv4, настроенные для адаптера.|
|Днссуффикслист|Коллекция String|Допустимые DNS-суффиксы для текущей сети. Например, Seattle.contoso.com|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
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
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
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





