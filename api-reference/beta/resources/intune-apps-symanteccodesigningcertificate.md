---
title: тип ресурса symantecCodeSigningCertificate
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ab178531c70be1a257a494024189cec2567408c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047186"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>тип ресурса symantecCodeSigningCertificate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получить symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Чтение свойств и связей [объекта symantecCodeSigningCertificate.](../resources/intune-apps-symanteccodesigningcertificate.md)|
|[Обновление symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Обновление свойств объекта [symantecCodeSigningCertificate.](../resources/intune-apps-symanteccodesigningcertificate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|содержимое|В двоичном формате|Сертификат Windows Symantec Code-Signing в формате необработанных данных.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|Состояние Cert Provisioned или not Provisioned. Возможные значения: `notProvisioned`, `provisioned`.|
|password|Строка|Пароль, необходимый для файла .pfx.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|String|Значение Subject для сертификата.|
|issuerName|String|Имя эмитента для сертификата.|
|эмитент|String|Значение Issuer для сертификата.|
|expirationDateTime|DateTimeOffset|Срок действия сертификата.|
|uploadDateTime|DateTimeOffset|Тип cert CodeSigning как Symantec Cert.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```



