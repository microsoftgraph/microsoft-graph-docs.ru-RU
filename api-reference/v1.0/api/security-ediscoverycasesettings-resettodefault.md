---
title: Сброс ediscoveryCaseSettings до значения по умолчанию
description: Сбросьте значение ediscoveryCaseSettingsobject до значений по умолчанию.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b7e73fb24aee0198ace5335c92fb07e1309e6bb0
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66840181"
---
# <a name="ediscoverycasesettings-resettodefault"></a>eDiscoveryCaseSettings: resetToDefault

Пространство имен: microsoft.graph.security



Сброс объекта [caseSettings](../resources/security-ediscoverycaseSettings.md) до значений по умолчанию.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/settings/resetToDefault
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "settings_resettodefault"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/settings/resettodefault
```
### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 200 OK
```
