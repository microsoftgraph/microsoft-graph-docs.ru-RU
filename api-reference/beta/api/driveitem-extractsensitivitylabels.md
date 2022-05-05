---
title: 'driveItem: extractSensitivityLabels'
description: Извлеките одну или несколько меток конфиденциальности, назначенных элементу диска.
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d516f6f530041d662f6818d5f8d832762678b038
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208890"
---
# <a name="driveitem-extractsensitivitylabels"></a>driveItem: extractSensitivityLabels
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлеките одну или несколько меток конфиденциальности, назначенных элементу диска, и обновите метаданные элемента диска, используя последние сведения о назначенной метке. В случае сбоя извлечения меток конфиденциальности файла возникает ошибка извлечения с соответствующим кодом ошибки и сообщением.

> **Примечание**. Этот API применим только к поддерживаемым расширениям файлов. При вызове этот API сначала получает метаданные метки конфиденциальности файла из базы данных, а затем проверяет, являются ли сведения метки конфиденциальности последними с точки зрения содержимого файла. Если да, возвращаются полученные из базы данных значения. Если нет, метки конфиденциальности извлекаются из потока содержимого файла, соответствующие метаданные обновляются в базе данных и возвращаются только что извлеченные значения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                             |
|:--------------------------------------|:--------------------------------------------------------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All                                        |
|Для приложений                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                                |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/extractSensitivityLabels
POST /drives/{drive-id}/root:/{item-path}/extractSensitivityLabels
POST /groups/{group-id}/drive/items/{item-id}/extractSensitivityLabels
POST /groups/{group-id}/drive/root:/{item-path}/extractSensitivityLabels
POST /me/drive/items/{item-id}/extractSensitivityLabels
POST /me/drive/root:/{item-path}/extractSensitivityLabels
POST /sites/{site-id}/drive/items/{item-id}/extractSensitivityLabels
POST /sites/{site-id}/drive/root:/{item-path}/extractSensitivityLabels
POST /users/{user-id}/drive/items/{item-id}/extractSensitivityLabels
POST /users/{user-id}/drive/root:/{item-path}/extractSensitivityLabels
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код `200 OK` отклика и объект [extractSensitivityLabelsResult](../resources/extractsensitivitylabelsresult.md) в теле отклика.

Помимо общих ошибок, которые относятся к Microsoft Graph, этот API `423 Locked` возвращает код ответа, указывающий, что доступ к файлу заблокирован. В таких случаях свойство **кода объекта** ответа указывает тип ошибки, который блокирует извлечение меток конфиденциальности.
Ниже приведены возможные значения для типов ошибок.

| Значение                       | Описание                                                                                                         |
|:----------------------------|:--------------------------------------------------------------------------------------------------------------------|
| fileDoubleKeyEncrypted      | Указывает, что файл защищен с помощью двойного шифрования ключей; поэтому его нельзя открыть для извлечения меток конфиденциальности.             |
| fileDecryptionNotSupported  | Указывает, что зашифрованный файл имеет определенные свойства, которые не позволяют открывать эти файлы SharePoint для извлечения меток конфиденциальности.    |
| fileDecryptionDeferred      | Указывает, что файл обрабатывается для расшифровки; поэтому его нельзя открыть для извлечения меток конфиденциальности.      |
| unknownFutureValue          | Значение sentinel для развиваемого перечисления. Не следует использовать.                                                                   |

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "extract-sensitivitylabels", "tags": "service.graph" } -->
``` http
POST https://graph.microsoft.com/beta/drive/root/items/016GVDAP3RCQS5VBQHORFIVU2ZMOSBL25U/extractSensitivityLabels
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/extract-sensitivitylabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/extract-sensitivitylabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extractSensitivityLabelsResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "microsoft.graph.extractSensitivityLabelsResult",
    "labels": [
      {
        "sensitivityLabelId": "5feba255-812e-446a-ac59-a7044ef827b5",
        "assignmentMethod": "standard",
        "tenantId": "fed495cb-8c27-41ea-8749-00b0a084bc3d"
      },
      {
        "sensitivityLabelId": "fa781fdf-68c8-43ec-ae08-c4813deb2144",
        "assignmentMethod": "standard",
        "tenantId": "277601b1-6094-456c-a358-95bfc99539d7"
      },
      {
        "sensitivityLabelId": "3937098d-df0c-4c8d-8f66-5876b57b75ba",
        "assignmentMethod": "standard",
        "tenantId": "f2477f30-c8a2-422d-8995-6f056b494655"
      }
    ]
  }
}
```

