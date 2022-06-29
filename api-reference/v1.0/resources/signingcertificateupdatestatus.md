---
title: Тип ресурса signingCertificateUpdateStatus
description: Предоставляет состояние последнего обновления сертификата подписи.
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 59129a7ce9d523c17fd4d497e91bf20da7af10b0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447458"
---
# <a name="signingcertificateupdatestatus-resource-type"></a>Тип ресурса signingCertificateUpdateStatus

Пространство имен: microsoft.graph

Предоставляет состояние и метку времени последнего обновления сертификата подписи. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|certificateUpdateResult|String|Состояние последнего обновления сертификата. Только для чтения. Список состояний см. в [разделе "Состояние certificateUpdateResult"](#certificateupdateresult-status).|
|lastRunDateTime|DateTimeOffset|Дата и время в формате ISO 8601 и время последнего обновления сертификата в формате UTC. Только для чтения. |

### <a name="certificateupdateresult-status"></a>Состояние certificateUpdateResult
| Значение | Описание |
| :--- | :--- |
|success|Попытка выполнена успешно.|
|unknownError|Не знаете причину сбоя.|
|internalServerError|Что-то пошло не так с нашей стороны.|
|noValidExistingCertFound|Действительный сертификат подписи не найден.|
|noStsAuthUrlFound|URL-адрес проверки подлинности STS не найден.|
|noFederationProtocolFound|Протокол федерации не найден.|
|noNewCertificateFound|Новый сертификат не найден.|
|couldNotAccessRemoteHost|Не удалось связаться с поставщиком, чтобы получить новые сертификаты.|
|connectionError|Произошла ошибка подключения|
|xmlParsingError|Не удалось проанализировать XML-код|
|badRequest|Получена ошибка BadRequest из запроса метаданных fed.|
|Несанкционированного|Получена неавторизованная ошибка из запроса метаданных федерации.|
|Запрещено|Получена ошибка "Запрещено" из запроса метаданных федерации.|
|notFound|Получена ошибка NotFound из запроса метаданных федерации.|
|providerError|Получено InternalServerError от поставщика.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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

