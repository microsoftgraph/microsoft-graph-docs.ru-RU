---
title: тип ресурсов сертификации
description: Представляет сведения о сертификации приложения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: arpitha-dhanapathi
ms.openlocfilehash: 6dedb9b58e3b59c707c6601fea12e9751ec3026f
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266437"
---
# <a name="certification-resource-type"></a>тип ресурсов сертификации

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сертификации [приложения.](application.md) 

Свойство сертификации приложения только для чтения и не может быть за установлено вручную. Он обновляется, когда приложение сертифицировано с помощью Microsoft 365 приложения. Дополнительные сведения см. [в Microsoft 365 App Compliance Program.](/microsoft-365-app-certification/docs/enterprise-app-certification-guide)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|certificationDetailsUrl|Строка|URL-адрес, отображает сведения о сертификации для приложения.|
|certificationExpirationDateTime|DateTimeOffset|Время истечения срока действия текущей сертификации для приложения.|
|isCertifiedByMicrosoft|Логическое|Указывает, сертифицировано ли приложение корпорацией Майкрософт.|
|isPublisherAttested|Логическое|Указывает, было ли приложение заверено разработчиком приложения или издателем.|
|lastCertificationDateTime|DateTimeOffset|Время, когда недавно была добавлена или обновлена сертификация для приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certification"
}-->

```json
{
  "isPublisherAttested": "Boolean",
  "isCertifiedByMicrosoft": "Boolean",
  "certificationDetailsUrl": "String",
  "lastCertificationDateTime": "DateTimeOffset",
  "certificationExpirationDateTime": "DateTimeOffset"
}
```
