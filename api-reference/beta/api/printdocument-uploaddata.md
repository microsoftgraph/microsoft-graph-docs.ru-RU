---
title: 'printDocument: Уплоаддата'
description: Отправьте один двоичный сегмент printDocument.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7592de07f74aa6fb715a90b2becad57a0e14b194
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896302"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="a5202-103">printDocument: Уплоаддата</span><span class="sxs-lookup"><span data-stu-id="a5202-103">printDocument: uploadData</span></span>

<span data-ttu-id="a5202-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5202-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5202-105">Отправьте один двоичный сегмент **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="a5202-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="a5202-106">Вы можете отправить файл целиком или разбить его на несколько диапазонов байтов, если число запросов не превышает 1 МБ.</span><span class="sxs-lookup"><span data-stu-id="a5202-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="a5202-107">Сегменты файла можно отправить в любом порядке и можно отправить параллельно, используя до четырех одновременных запросов.</span><span class="sxs-lookup"><span data-stu-id="a5202-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="a5202-108">После отправки всех двоичных сегментов документа двоичный файл связывается с **методом printJob**.</span><span class="sxs-lookup"><span data-stu-id="a5202-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5202-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5202-109">Permissions</span></span>
<span data-ttu-id="a5202-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5202-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a5202-112">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="a5202-112">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="a5202-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5202-113">Permission type</span></span> | <span data-ttu-id="a5202-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5202-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a5202-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5202-115">Delegated (work or school account)</span></span>| <span data-ttu-id="a5202-116">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a5202-116">Users.Read.All</span></span> |
|<span data-ttu-id="a5202-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5202-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5202-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5202-118">Not Supported.</span></span>|
|<span data-ttu-id="a5202-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a5202-119">Application</span></span>|<span data-ttu-id="a5202-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5202-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5202-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5202-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="a5202-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5202-122">Request headers</span></span>
| <span data-ttu-id="a5202-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a5202-123">Name</span></span>          | <span data-ttu-id="a5202-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a5202-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a5202-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5202-125">Authorization</span></span> | <span data-ttu-id="a5202-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5202-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5202-128">Диапазон</span><span class="sxs-lookup"><span data-stu-id="a5202-128">Range</span></span> | <span data-ttu-id="a5202-129">байт = {Стартбитеиндекс} — {Ендбитеиндекс}</span><span class="sxs-lookup"><span data-stu-id="a5202-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="a5202-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="a5202-130">Content-Length</span></span> | <span data-ttu-id="a5202-131">ContentLength</span><span class="sxs-lookup"><span data-stu-id="a5202-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="a5202-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5202-132">Content-type</span></span>  | <span data-ttu-id="a5202-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5202-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5202-135">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5202-135">Request body</span></span>
<span data-ttu-id="a5202-136">Текст запроса представляет собой двоичный объект BLOB, содержащий байты документа, которые задаются в `Range` заголовке как инклюзивный диапазон байтов.</span><span class="sxs-lookup"><span data-stu-id="a5202-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="a5202-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5202-137">Response</span></span>
<span data-ttu-id="a5202-138">В случае успешного выполнения этот метод возвращает один из следующих ответов.</span><span class="sxs-lookup"><span data-stu-id="a5202-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="a5202-139">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a5202-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="a5202-140">Условие</span><span class="sxs-lookup"><span data-stu-id="a5202-140">Condition</span></span>     | <span data-ttu-id="a5202-141">Код ответа</span><span class="sxs-lookup"><span data-stu-id="a5202-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="a5202-142">Один или несколько двоичных сегментов по-прежнему необходимо отправить</span><span class="sxs-lookup"><span data-stu-id="a5202-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="a5202-143">Все двоичные сегменты успешно отправлены</span><span class="sxs-lookup"><span data-stu-id="a5202-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="a5202-144">Пример</span><span class="sxs-lookup"><span data-stu-id="a5202-144">Example</span></span>
<span data-ttu-id="a5202-145">В приведенном ниже примере показано, как вызвать этот API, чтобы отправить первые 72797 байтов документа.</span><span class="sxs-lookup"><span data-stu-id="a5202-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="a5202-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5202-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
##### <a name="response"></a><span data-ttu-id="a5202-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5202-147">Response</span></span>

<span data-ttu-id="a5202-148">Отсутствует один или несколько сегментов:</span><span class="sxs-lookup"><span data-stu-id="a5202-148">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="a5202-149">Все принимаемые сегменты:</span><span class="sxs-lookup"><span data-stu-id="a5202-149">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```