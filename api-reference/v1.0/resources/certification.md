---
title: Тип ресурса сертификации
description: Представляет сведения о сертификации приложения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: arpitha-dhanapathi
ms.openlocfilehash: 228670677eb8d618803bb86594a3cd95cf3f2e0d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096327"
---
# <a name="certification-resource-type"></a>Тип ресурса сертификации
Пространство имен: microsoft.graph

Представляет сведения о сертификации [приложения](application.md). 

Свойство сертификации приложения доступно только для чтения и не может быть задано вручную. Он обновляется, когда приложение сертифицировано с помощью Microsoft 365 соответствия требованиям приложений. Дополнительные сведения см[. в Microsoft 365 App Compliance Program](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|certificationDetailsUrl|Строка|URL-адрес, показывающий сведения о сертификации для приложения.|
|certificationExpirationDateTime|DateTimeOffset|Метка времени истечения срока действия текущей сертификации для приложения.|
|isCertifiedByMicrosoft|Boolean|Указывает, сертифицировано ли приложение корпорацией Майкрософт.|
|isPublisherAttested|Boolean|Указывает, было ли приложение самозаверяющееся разработчиком или издателем.|
|lastCertificationDateTime|DateTimeOffset|Метка времени последнего добавления или обновления сертификации для приложения.|

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
