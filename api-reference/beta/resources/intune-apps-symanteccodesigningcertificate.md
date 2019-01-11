---
title: Тип ресурса symantecCodeSigningCertificate
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a2e4f53e0ca7329f163b507677e2b91a4c02fe12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845012"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>Тип ресурса symantecCodeSigningCertificate

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md);|Чтение свойства и связи объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|
|[Обновление symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md);|Обновление свойства объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|content|Binary|Сертификат подписи кода Symantec Windows в формате необработанные данные.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|Состояние Cert подготовить к работе или не подготовлен. Возможные значения: `notProvisioned`, `provisioned`.|
|password|Строка|Пароль, необходимый для PFX-файл.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|Строка|Значения субъектов для сертификата.|
|Имя поставщика|Строка|Имя поставщика для сертификата.|
|издателя|Строка|Значение издателя сертификата.|
|expirationDateTime|DateTimeOffset|Срок действия сертификата.|
|uploadDateTime|DateTimeOffset|Тип сертификата подписывания кода как Symantec Cert.|

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





