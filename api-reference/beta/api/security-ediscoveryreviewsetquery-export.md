---
title: 'ediscoveryReviewSetQuery: экспорт'
description: Инициируйте экспорт из запроса reviewSet.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: aefa42a52c9b9619db9c3fd4c7a499d8961db39f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946391"
---
# <a name="ediscoveryreviewsetquery-export"></a>ediscoveryReviewSetQuery: экспорт
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инициируйте экспорт из **запроса reviewSet** .  Дополнительные сведения см. в статье "Экспорт документов [из набора для проверки в Advanced eDiscovery"](/microsoft-365/compliance/export-documents-from-review-set).


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|


## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries/{queryId}/export
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление параметров в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|outputName|Строка| Имя экспорта. Обязательный. |
|description|Строка| Описание экспорта |
|azureBlobContainer|Строка| При экспорте в собственную учетную запись хранения Azure это URL-адрес контейнера. |
|azureBlobToken|Строка| При экспорте в собственную учетную запись хранения Azure маркер SAS для URL-адреса контейнера. |
|exportOptions|Строка|Задает параметры, которые могут управлять форматом экспорта. Возможные значения: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|Строка| Параметры, которые контролирует структуру файлов и упаковку экспорта. Возможные значения: `none`, `directory`, `pst`.|


## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetquerythis.export"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries/fcb86cd1-50e0-427c-840e-ba6f087364e5/export
Content-Type: application/json

{
    "outputName": "Export reviewset query via API",
    "description": "Export for the Contoso investigation 2",
    "exportOptions": "originalFiles,fileInfo,tags",
    "exportStructure": "directory"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
