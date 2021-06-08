---
title: Как получить фотографию группы
description: Вы можете получить фотографию (изображение) для группы.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: af4e5a95f4af666210be098eb20836bc713d9a8b
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787164"
---
# <a name="get-team-photo"></a><span data-ttu-id="bdb7f-103">Как получить фотографию группы</span><span class="sxs-lookup"><span data-stu-id="bdb7f-103">Get team photo</span></span>

<span data-ttu-id="bdb7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdb7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdb7f-105">Вы можете получить фотографию (изображение) для группы или метаданные этой фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-105">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="bdb7f-106">В целом, лучше всего сначала попробовать извлечь метаданные о размере фотографии, которую вы хотите получить, чтобы убедиться в том, что этот размер доступен.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-106">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="bdb7f-107">После того как вы извлекли метаданные, используйте путь `/$value`, чтобы получить двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-107">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="bdb7f-108">Действуя этим методом, мы сначала пробуем извлечь указанную фотографию из Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-108">This method first attempts to retrieve the specified photo from Microsoft 365.</span></span> <span data-ttu-id="bdb7f-109">Если фотография недоступна в Microsoft 365, производится попытка извлечь ее из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-109">If the photo is not available in Microsoft 365, it attempts to retrieve the photo from Azure Active Directory instead.</span></span>

<span data-ttu-id="bdb7f-110">Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-110">The following are the supported sizes of HD photos in Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="bdb7f-111">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-111">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="bdb7f-112">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для фотографии этого размера.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-112">You can get the metadata of the largest available photo, or optionally specify a size to get the metadata for that photo size.</span></span> <span data-ttu-id="bdb7f-113">Если запрашиваемый размер недоступен, вы можете получить фотографию меньшего размера.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-113">If the size you request is not available, you can still get a smaller size.</span></span> <span data-ttu-id="bdb7f-114">Например, если самая крупная загруженная фотография имеет размер 504 x 504 пикселя, для скачивания будут доступны все размеры этой фотографии, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-114">For example, if the largest photo uploaded is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span> <span data-ttu-id="bdb7f-115">Если указанный размер недоступен в Microsoft 365 или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-115">If the specified size is not available in the Microsoft 365 or in Azure Active Directory, the size 1x1 is returned with the rest of the metadata.</span></span>

> [!Note]
> <span data-ttu-id="bdb7f-116">Общий размер запроса REST не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-116">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="bdb7f-117">Таким образом, размер фотографии составит менее 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-117">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdb7f-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdb7f-118">Permissions</span></span>

<span data-ttu-id="bdb7f-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdb7f-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdb7f-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdb7f-121">Permission type</span></span>      | <span data-ttu-id="bdb7f-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdb7f-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdb7f-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdb7f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="bdb7f-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdb7f-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bdb7f-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdb7f-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdb7f-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-126">Not supported.</span></span>    |
|<span data-ttu-id="bdb7f-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdb7f-127">Application</span></span> | <span data-ttu-id="bdb7f-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-128">Not supported.</span></span> |

> <span data-ttu-id="bdb7f-129">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bdb7f-129">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="bdb7f-p107">**Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-p107">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bdb7f-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdb7f-132">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="bdb7f-133">Как получить метаданные фотографии</span><span class="sxs-lookup"><span data-stu-id="bdb7f-133">Get the metadata of the photo</span></span>

<span data-ttu-id="bdb7f-134">Эта конечная точка возвращает метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-134">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="bdb7f-135">Если размер не указывать, возвращаются метаданные крупнейшей доступной фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-135">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="bdb7f-136">Как получить фотографию</span><span class="sxs-lookup"><span data-stu-id="bdb7f-136">Get the photo</span></span>

<span data-ttu-id="bdb7f-137">Эта конечная точка извлекает двоичные данные для фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-137">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="bdb7f-138">Если размер не указан, возвращается наибольший доступный размер.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-138">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="bdb7f-139">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="bdb7f-139">Path parameters</span></span>

<span data-ttu-id="bdb7f-140">Для этого метода поддерживается необязательный параметр пути, позволяющий указать размер фотографии, которую нужно извлечь.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-140">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="bdb7f-141">Можно указать любой размер вплоть до максимального доступного.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-141">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="bdb7f-142">Чтобы определить максимальный доступный размер, получите метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-142">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="bdb7f-143">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="bdb7f-143">**Parameter**</span></span>|<span data-ttu-id="bdb7f-144">**Тип**</span><span class="sxs-lookup"><span data-stu-id="bdb7f-144">**Type**</span></span>|<span data-ttu-id="bdb7f-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bdb7f-145">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bdb7f-146">size</span><span class="sxs-lookup"><span data-stu-id="bdb7f-146">size</span></span>  |<span data-ttu-id="bdb7f-147">String</span><span class="sxs-lookup"><span data-stu-id="bdb7f-147">String</span></span>  | <span data-ttu-id="bdb7f-148">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-148">A photo size.</span></span> <span data-ttu-id="bdb7f-149">Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-149">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="bdb7f-150">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-150">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="bdb7f-151">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-151">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="bdb7f-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdb7f-152">Request headers</span></span>

| <span data-ttu-id="bdb7f-153">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdb7f-153">Header</span></span>        | <span data-ttu-id="bdb7f-154">Значение</span><span class="sxs-lookup"><span data-stu-id="bdb7f-154">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="bdb7f-155">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdb7f-155">Authorization</span></span> | <span data-ttu-id="bdb7f-p112">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-p112">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bdb7f-158">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdb7f-158">Request body</span></span>

<span data-ttu-id="bdb7f-159">Текст для этого запроса указывать не нужно.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-159">Do not supply a body for this request.</span></span>

## <a name="response"></a><span data-ttu-id="bdb7f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdb7f-160">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="bdb7f-161">Отклик при получении метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="bdb7f-161">Response for getting the metadata of a photo</span></span>

<span data-ttu-id="bdb7f-162">При успешной отправке запроса этим способом возвращаются код отклика`200 OK` и метаданные о запрашиваемой фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-162">If successful, this method returns a `200 OK` response code, and metadata about the photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="bdb7f-163">Отклик при получении фотографии</span><span class="sxs-lookup"><span data-stu-id="bdb7f-163">Response for getting the photo</span></span>

<span data-ttu-id="bdb7f-164">При успешной отправке запроса этим способом возвращаются код отклика `200 OK` и двоичные данные запрашиваемой фотографии.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-164">If successful, this method returns a `200 OK` response code, and the binary data for the photo.</span></span>

## <a name="examples"></a><span data-ttu-id="bdb7f-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="bdb7f-165">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="bdb7f-166">Пример 1. Как получить метаданные фотографии</span><span class="sxs-lookup"><span data-stu-id="bdb7f-166">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="bdb7f-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdb7f-167">Request</span></span>

<span data-ttu-id="bdb7f-168">Ниже приведен пример запроса на получение метаданных фотографии группы.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-168">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="bdb7f-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdb7f-169">Response</span></span>

<span data-ttu-id="bdb7f-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-170">Here is an example of the response.</span></span>

> <span data-ttu-id="bdb7f-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="bdb7f-172">Пример 2. Как получить фотографию группы определенного размера</span><span class="sxs-lookup"><span data-stu-id="bdb7f-172">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="bdb7f-173">Вот пример запроса на получение фотографии группы определенного размера.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-173">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="bdb7f-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdb7f-174">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="bdb7f-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdb7f-175">Response</span></span>

<span data-ttu-id="bdb7f-176">Содержит двоичные данные запрошенной фотографии размера 240 х 240.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-176">Contains the binary data of the requested 240x240 photo.</span></span> <span data-ttu-id="bdb7f-177">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="bdb7f-177">The HTTP response code is 200.</span></span>

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


