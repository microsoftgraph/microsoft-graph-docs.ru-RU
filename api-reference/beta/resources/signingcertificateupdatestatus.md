---
title: Тип ресурса signingCertificateUpdateStatus
description: Предоставляет состояние последнего обновления сертификата подписи.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 108b5169ac9b043e4ce2a80f5c620a266d391338
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2022
ms.locfileid: "64852733"
---
# <a name="signingcertificateupdatestatus-resource-type"></a>Тип ресурса signingCertificateUpdateStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет состояние и метку времени последнего обновления сертификата подписи. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|certificateUpdateResult|String|Состояние последнего обновления сертификата. Только для чтения. Список состояний см. в [разделе "Состояние certificateUpdateResult"](#certificateupdateresult-status).|
|lastRunDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и время последнего обновления сертификата в формате UTC. Только для чтения. |

### <a name="certificateupdateresult-status"></a>Состояние certificateUpdateResult
| Значение | Описание |
| :--- | :--- |
|success|Операция обновления сертификата прошла успешно.|
|unknownError|Причина сбоя не определена.|
|internalServerError|При обработке запроса возникла внутренняя ошибка сервера.|
|noValidExistingCertFound|Действительный сертификат подписи не найден.|
|noStsAuthUrlFound|URL-адрес проверки подлинности STS не найден.|
|noFederationProtocolFound|Протокол федерации не определен.|
|noNewCertificateFound|Новый сертификат не найден.|
|couldNotAccessRemoteHost|Не удалось связаться с поставщиком, чтобы получить новые сертификаты.|
|connectionError|Произошла ошибка подключения, например истекло время ожидания подключения.|
|xmlParsingError|Не удалось проанализировать XML-код.|
|badRequest|Получен код `400 BadRequest` ошибки в запросе метаданных fed.|
|Несанкционированного|Получен `401 Unauthorized` код ошибки в запросе метаданных fed.|
|Запрещено|Получен `403 Forbidden` код ошибки в запросе метаданных fed.|
|notFound|Получен `404 NotFound` код ошибки в запросе метаданных fed.|
|providerError|Получен код `500 InternalServerError` ошибки от поставщика.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.signingCertificateUpdateStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signingCertificateUpdateStatus",
  "certificateUpdateResult": "String",
  "lastRunDateTime": "String (timestamp)"
}
```

