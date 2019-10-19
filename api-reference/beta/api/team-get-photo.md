---
title: Как получить фотографию группы
description: Вы можете получить фотографию (изображение) для группы.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ab94922ed34b01be43a7776f017341a2b47f474d
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2019
ms.locfileid: "37598235"
---
# <a name="get-team-photo"></a><span data-ttu-id="bc0b8-103">Как получить фотографию группы</span><span class="sxs-lookup"><span data-stu-id="bc0b8-103">Get team photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc0b8-104">Вы можете получить фотографию (изображение) для группы или метаданные этой фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-104">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="bc0b8-105">В целом, лучше всего сначала попробовать извлечь метаданные о размере фотографии, которую вы хотите получить, чтобы убедиться в том, что этот размер доступен.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-105">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="bc0b8-106">После того как вы извлекли метаданные, используйте путь `/$value`, чтобы получить двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-106">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="bc0b8-107">Действуя этим методом, мы сначала пробуем извлечь указанную фотографию из Office 365.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-107">This method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="bc0b8-108">Если фотография недоступна в Office 365, производится попытка извлечь ее из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-108">If the photo is not available in Office 365, it attempts to retrieve the photo from Azure Active Directory instead.</span></span>

<span data-ttu-id="bc0b8-109">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-109">The following are the supported sizes of HD photos in Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="bc0b8-110">Фотографии, хранящиеся в Azure Active Directory, могут быть любого размера.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-110">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="bc0b8-111">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для фотографии этого размера.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-111">You can get the metadata of the largest available photo, or optionally specify a size to get the metadata for that photo size.</span></span> <span data-ttu-id="bc0b8-112">Если запрашиваемый размер недоступен, вы можете получить фотографию меньшего размера.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-112">If the size you request is not available, you can still get a smaller size.</span></span> <span data-ttu-id="bc0b8-113">Например, если самая крупная загруженная фотография имеет размер 504 x 504 пикселя, для скачивания будут доступны все размеры этой фотографии, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-113">For example, if the largest photo uploaded is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span> <span data-ttu-id="bc0b8-114">Если указанный размер недоступен в Office 365 или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-114">If the specified size is not available in the Office 365 or in Azure Active Directory, the size 1x1 is returned with the rest of the metadata.</span></span>

> [!Note]
> <span data-ttu-id="bc0b8-115">Общий размер запроса REST не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-115">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="bc0b8-116">Таким образом, размер фотографии составит менее 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-116">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc0b8-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc0b8-117">Permissions</span></span>

<span data-ttu-id="bc0b8-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc0b8-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc0b8-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc0b8-120">Permission type</span></span>      | <span data-ttu-id="bc0b8-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc0b8-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc0b8-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc0b8-122">Delegated (work or school account)</span></span> | <span data-ttu-id="bc0b8-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0b8-123">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc0b8-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc0b8-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc0b8-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-125">Not supported.</span></span>    |
|<span data-ttu-id="bc0b8-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc0b8-126">Application</span></span> | <span data-ttu-id="bc0b8-127">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0b8-127">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc0b8-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc0b8-128">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="bc0b8-129">Как получить метаданные фотографии</span><span class="sxs-lookup"><span data-stu-id="bc0b8-129">Get the metadata of the photo</span></span>

<span data-ttu-id="bc0b8-130">Эта конечная точка возвращает метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-130">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="bc0b8-131">Если размер не указывать, возвращаются метаданные крупнейшей доступной фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-131">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo
GET /beta/teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="bc0b8-132">Как получить фотографию</span><span class="sxs-lookup"><span data-stu-id="bc0b8-132">Get the photo</span></span>

<span data-ttu-id="bc0b8-133">Эта конечная точка извлекает двоичные данные для фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-133">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="bc0b8-134">Если размер не указан, возвращается наибольший доступный размер.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-134">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="bc0b8-135">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="bc0b8-135">Path parameters</span></span>

<span data-ttu-id="bc0b8-136">Для этого метода поддерживается необязательный параметр пути, позволяющий указать размер фотографии, которую нужно извлечь.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-136">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="bc0b8-137">Можно указать любой размер вплоть до максимального доступного.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-137">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="bc0b8-138">Чтобы определить максимальный доступный размер, получите метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-138">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="bc0b8-139">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="bc0b8-139">**Parameter**</span></span>|<span data-ttu-id="bc0b8-140">**Тип**</span><span class="sxs-lookup"><span data-stu-id="bc0b8-140">**Type**</span></span>|<span data-ttu-id="bc0b8-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc0b8-141">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bc0b8-142">size</span><span class="sxs-lookup"><span data-stu-id="bc0b8-142">size</span></span>  |<span data-ttu-id="bc0b8-143">String</span><span class="sxs-lookup"><span data-stu-id="bc0b8-143">String</span></span>  | <span data-ttu-id="bc0b8-144">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-144">A photo size.</span></span> <span data-ttu-id="bc0b8-145">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-145">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="bc0b8-146">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-146">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="bc0b8-147">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-147">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="bc0b8-148">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc0b8-148">Request headers</span></span>

| <span data-ttu-id="bc0b8-149">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc0b8-149">Header</span></span>        | <span data-ttu-id="bc0b8-150">Значение</span><span class="sxs-lookup"><span data-stu-id="bc0b8-150">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="bc0b8-151">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc0b8-151">Authorization</span></span> | <span data-ttu-id="bc0b8-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-p111">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc0b8-154">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc0b8-154">Request body</span></span>

<span data-ttu-id="bc0b8-155">Текст для этого запроса указывать не нужно.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-155">Do not supply a body for this request.</span></span>

## <a name="response"></a><span data-ttu-id="bc0b8-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc0b8-156">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="bc0b8-157">Отклик при получении метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="bc0b8-157">Response for getting the metadata of a photo</span></span>

<span data-ttu-id="bc0b8-158">При успешной отправке запроса этим способом возвращаются код отклика`200 OK` и метаданные о запрашиваемой фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-158">If successful, this method returns a `200 OK` response code, and metadata about the photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="bc0b8-159">Отклик при получении фотографии</span><span class="sxs-lookup"><span data-stu-id="bc0b8-159">Response for getting the photo</span></span>

<span data-ttu-id="bc0b8-160">При успешной отправке запроса этим способом возвращаются код отклика `200 OK` и двоичные данные запрашиваемой фотографии.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-160">If successful, this method returns a `200 OK` response code, and the binary data for the photo.</span></span>

## <a name="examples"></a><span data-ttu-id="bc0b8-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="bc0b8-161">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="bc0b8-162">Пример 1. Как получить метаданные фотографии</span><span class="sxs-lookup"><span data-stu-id="bc0b8-162">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="bc0b8-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc0b8-163">Request</span></span>

<span data-ttu-id="bc0b8-164">Ниже приведен пример запроса на получение метаданных фотографии группы.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-164">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="bc0b8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc0b8-165">Response</span></span>

<span data-ttu-id="bc0b8-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-166">Here is an example of the response.</span></span>

> <span data-ttu-id="bc0b8-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="bc0b8-169">Пример 2. Как получить фотографию группы определенного размера</span><span class="sxs-lookup"><span data-stu-id="bc0b8-169">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="bc0b8-170">Вот пример запроса на получение фотографии группы определенного размера.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-170">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="bc0b8-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc0b8-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="bc0b8-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc0b8-172">Response</span></span>

<span data-ttu-id="bc0b8-173">Содержит двоичные данные запрошенной фотографии размера 240 х 240.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-173">Contains the binary data of the requested 240x240 photo.</span></span> <span data-ttu-id="bc0b8-174">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-174">The HTTP response code is 200.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
