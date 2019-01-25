---
title: Тип ресурса onPremisesPublishing
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508183"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="aeb15-103">Тип ресурса onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="aeb15-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="aeb15-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="aeb15-104">Properties</span></span>
| <span data-ttu-id="aeb15-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="aeb15-105">Property</span></span>     | <span data-ttu-id="aeb15-106">Тип</span><span class="sxs-lookup"><span data-stu-id="aeb15-106">Type</span></span>   |<span data-ttu-id="aeb15-107">Описание</span><span class="sxs-lookup"><span data-stu-id="aeb15-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aeb15-108">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="aeb15-108">customDomainCertificate</span></span>|<span data-ttu-id="aeb15-109">String</span><span class="sxs-lookup"><span data-stu-id="aeb15-109">String</span></span>|<span data-ttu-id="aeb15-110">Сведения о сертификате, связанных с приложением, при использовании настраиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="aeb15-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="aeb15-111">Использование домена по умолчанию значение NULL.</span><span class="sxs-lookup"><span data-stu-id="aeb15-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="aeb15-112">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="aeb15-112">externalAuthenticationType</span></span>|<span data-ttu-id="aeb15-113">String</span><span class="sxs-lookup"><span data-stu-id="aeb15-113">String</span></span>|<span data-ttu-id="aeb15-114">Дополнительные сведения об значение предварительной проверки подлинности для приложения возможными значениями являются: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="aeb15-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="aeb15-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="aeb15-115">externalUrl</span></span>|<span data-ttu-id="aeb15-116">String</span><span class="sxs-lookup"><span data-stu-id="aeb15-116">String</span></span>|<span data-ttu-id="aeb15-117">Опубликованные внешний URL-адрес для приложения.</span><span class="sxs-lookup"><span data-stu-id="aeb15-117">The published external url for the application.</span></span> <span data-ttu-id="aeb15-118">Пример:</span><span class="sxs-lookup"><span data-stu-id="aeb15-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="aeb15-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="aeb15-119">internalUrl</span></span>|<span data-ttu-id="aeb15-120">String</span><span class="sxs-lookup"><span data-stu-id="aeb15-120">String</span></span>|<span data-ttu-id="aeb15-121">Внутренний URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="aeb15-121">The internal url of the application.</span></span> <span data-ttu-id="aeb15-122">Пример:</span><span class="sxs-lookup"><span data-stu-id="aeb15-122">For example https://intranet/</span></span> |
|<span data-ttu-id="aeb15-123">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="aeb15-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="aeb15-124">Логическое</span><span class="sxs-lookup"><span data-stu-id="aeb15-124">Boolean</span></span>|<span data-ttu-id="aeb15-125">Указывает, если приложение публикуется в настоящее время или нет.</span><span class="sxs-lookup"><span data-stu-id="aeb15-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="aeb15-126">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="aeb15-126">applicationServerTimeout</span></span>|<span data-ttu-id="aeb15-127">String</span><span class="sxs-lookup"><span data-stu-id="aeb15-127">String</span></span>|<span data-ttu-id="aeb15-128">Во время выполнения соединитель будет ожидать ответа из базы данных приложения до закрытия подключения.</span><span class="sxs-lookup"><span data-stu-id="aeb15-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="aeb15-129">Возможные значения: `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="aeb15-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="aeb15-130">Использование `long` Если сервер принимает более 60 75 секунд отвечать на запросы.</span><span class="sxs-lookup"><span data-stu-id="aeb15-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="aeb15-131">Также попробуйте `long` Если вы не можете получить доступ к приложению и состояние ошибки «Время ожидания базы данных».</span><span class="sxs-lookup"><span data-stu-id="aeb15-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="aeb15-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="aeb15-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="aeb15-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="aeb15-133">Boolean</span></span>|<span data-ttu-id="aeb15-134">Указывает, если приложение следует перевести URL-адреса в заголовке ответа.</span><span class="sxs-lookup"><span data-stu-id="aeb15-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="aeb15-135">Этот компонент включает Установка правильное веб-узла для файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="aeb15-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aeb15-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aeb15-136">JSON representation</span></span>

<span data-ttu-id="aeb15-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aeb15-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
