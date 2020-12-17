---
title: Обновление конфигурации printJob
description: Обновление конфигурации задания печати
author: tomsato-ms
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23d61d24367bc5c69d4613ac30deed9244a5ac08
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706391"
---
# <a name="update-printjob-configuration"></a><span data-ttu-id="f5489-103">Обновление конфигурации printJob</span><span class="sxs-lookup"><span data-stu-id="f5489-103">Update printJob configuration</span></span>

<span data-ttu-id="f5489-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5489-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5489-105">Обновление свойства [конфигурации](../resources/printjobconfiguration.md) задания [печати.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="f5489-105">Update the [configuration](../resources/printjobconfiguration.md) property of a [print job](../resources/printjob.md).</span></span>

<span data-ttu-id="f5489-106">Для обновления конфигурации задания печати необходимо, чтобы задание печати было в состоянии "удерживания" путем регистрации триггера задачи для принтера.</span><span class="sxs-lookup"><span data-stu-id="f5489-106">Updating a print job configuration requires the print job to be in a held state by registering a task trigger for the printer.</span></span> <span data-ttu-id="f5489-107">Подробные сведения о регистрации триггера задачи см. в подзадаче "Расширение универсальной печати [для поддержки печати с потягивом".](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="f5489-107">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5489-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5489-108">Permissions</span></span>
<span data-ttu-id="f5489-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5489-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f5489-111">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть [](printer-get.md) активная подписка универсальной печати, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f5489-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="f5489-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5489-112">Permission type</span></span> | <span data-ttu-id="f5489-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5489-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f5489-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5489-114">Delegated (work or school account)</span></span>| <span data-ttu-id="f5489-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5489-115">Not supported.</span></span> |
|<span data-ttu-id="f5489-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5489-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5489-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5489-117">Not Supported.</span></span>|
|<span data-ttu-id="f5489-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="f5489-118">Application</span></span>| <span data-ttu-id="f5489-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f5489-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5489-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5489-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}/configuration
```
## <a name="request-headers"></a><span data-ttu-id="f5489-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5489-121">Request headers</span></span>
| <span data-ttu-id="f5489-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f5489-122">Name</span></span>          | <span data-ttu-id="f5489-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f5489-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f5489-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5489-124">Authorization</span></span> | <span data-ttu-id="f5489-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5489-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5489-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5489-127">Request body</span></span>
<span data-ttu-id="f5489-128">В теле запроса укажийте значения соответствующих полей [printJobConfiguration.](../resources/printjobconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5489-128">In the request body, supply the values of the relevant [printJobConfiguration](../resources/printjobconfiguration.md) fields.</span></span> <span data-ttu-id="f5489-129">Существующие свойства, не включенные в тело запроса, сохраняют свои прежние значения.</span><span class="sxs-lookup"><span data-stu-id="f5489-129">Existing properties that are not included in the request body will maintain their previous values.</span></span>

## <a name="response"></a><span data-ttu-id="f5489-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5489-130">Response</span></span>
<span data-ttu-id="f5489-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5489-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f5489-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f5489-132">Example</span></span>
<span data-ttu-id="f5489-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f5489-133">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="f5489-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5489-134">Request</span></span>
<span data-ttu-id="f5489-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5489-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-update-configuration"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration

{
  "feedOrientation": "longEdgeFirst",
  "pageRanges": [
    {
      "start": 1,
      "end": 1
    }
  ],
  "quality": "medium",
  "dpi": 600,
  "orientation": "landscape",
  "copies": 1,
  "duplexMode": "oneSided",
  "colorMode": "blackAndWhite",
  "inputBin": "by-pass-tray",
  "outputBin": "output-tray",
  "mediaSize": "A4",
  "margin": {
    "top": 0,
    "bottom": 0,
    "left": 0,
    "right": 0
  },
  "mediaType": "stationery",
  "finishings": null,
  "pagesPerSheet": 1,
  "multipageLayout": "clockwiseFromBottomLeft",
  "collate": false,
  "scaling": "shrinkToFit",
  "fitPdfToPage": false
}
```

### <a name="response"></a><span data-ttu-id="f5489-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5489-136">Response</span></span>
<span data-ttu-id="f5489-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5489-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


