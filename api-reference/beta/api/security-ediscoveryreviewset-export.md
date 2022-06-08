---
title: 'ediscoveryReviewSet: экспорт'
description: Инициируйте экспорт из reviewSet.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 344f8ffcce3221489adaf59665f5fe5d0ec35fc2
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946401"
---
# <a name="ediscoveryreviewset-export"></a>ediscoveryReviewSet: экспорт
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инициируйте экспорт из **reviewSet**.  Дополнительные сведения см. в статье "Экспорт документов [из набора для проверки в Advanced eDiscovery"](/microsoft-365/compliance/export-documents-from-review-set).


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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/export
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

Если экспорт успешно запущен, это действие возвращает код `202 Accepted` отклика. Ответ также будет содержать заголовок `Location` , содержащий расположение операции [экспорта,](../resources/security-ediscoveryexportoperation.md) созданной для обработки экспорта.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetthis.export"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/export
Content-Type: application/json

{
    "outputName": "Export via API",
    "description": "Export for the Contoso investigation",
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

