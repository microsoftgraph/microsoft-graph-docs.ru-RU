---
title: Создание windows10XTrustedRootCertificate
description: Создание нового объекта windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b8a8995988a0eedd2f8204db12c9eb4ded184d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242419"
---
# <a name="create-windows10xtrustedrootcertificate"></a>Создание windows10XTrustedRootCertificate

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта windows10XTrustedRootCertificate в формате JSON.

В следующей таблице приведены свойства, необходимые при создании windows10XTrustedRootCertificate.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор профиля унаследован от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|version|Int32|Версия профиля, унаследованного от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|Отображаемое имя профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|String|Описание профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|креатиондатетиме|DateTimeOffset|Создан профиль DateTime, наследуемый от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение профиля DateTime унаследовано от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|Коллекция строк|Теги областей унаследованы от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|trustedRootCertificate|Binary|Доверенный корневой сертификат|
|цертфиленаме|String|Имя файла, отображаемое в пользовательском интерфейсе.|
|дестинатионсторе|[цертификатедестинатионсторе](../resources/intune-shared-certificatedestinationstore.md)|Расположение хранилища назначения для доверенного корневого сертификата. Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 456

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 569

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "be0bfd01-fd01-be0b-01fd-0bbe01fd0bbe",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




