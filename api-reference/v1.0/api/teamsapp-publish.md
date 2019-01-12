---
title: Permissions
description: 'Публикация приложения в каталоге приложений группами Майкрософт. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7faf5847b78d6221b5167c775def75ae9a2ce629
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911877"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a>Публикация приложений в каталоге приложений организации



Публикация [приложения](../resources/teamsapp.md) в каталог приложений группами Майкрософт. В частности этот интерфейс API публикует приложение в каталоге организации (клиент каталога приложений); созданный ресурс будет иметь `distributionMethod`  =  `organization`.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Примечание:** Только глобальный администратор может вызывать этот интерфейс API. 

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись)     | AppCatalog.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается|
| Для приложений                            | Не поддерживается|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type  | приложение/zip |

## <a name="request-body"></a>Тело запроса

Zip полезных команд манифеста. Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). Не удается создать приложения для организации, которая имеет тот же идентификатор манифеста в качестве другого приложения в организации.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [teamsCatalogApp](../resources/teamsapp.md) .

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Сведения о создании ZIP-файл приложения группами Майкрософт перейдите в раздел [Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). 

### <a name="response"></a>Ответ

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
