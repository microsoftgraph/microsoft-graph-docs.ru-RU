---
title: Тип ресурса educationSynchronizationConnectionSettings
description: 'Представляет параметры подключения поставщика. Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526867"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="1b162-104">Тип ресурса educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="1b162-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b162-105">Представляет параметры подключения поставщика.</span><span class="sxs-lookup"><span data-stu-id="1b162-105">Represents the provider connection settings.</span></span> <span data-ttu-id="1b162-106">Это позволяет системы, чтобы знать, как для подключения к поставщику API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="1b162-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="1b162-107">**Примечание:** В данном сложном типе абстрактный.</span><span class="sxs-lookup"><span data-stu-id="1b162-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="1b162-108">Обращайтесь к определенным типам параметров подключения из списка.</span><span class="sxs-lookup"><span data-stu-id="1b162-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="1b162-109">Производные типы</span><span class="sxs-lookup"><span data-stu-id="1b162-109">Derived types</span></span>
| <span data-ttu-id="1b162-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1b162-110">Type</span></span> | <span data-ttu-id="1b162-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1b162-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="1b162-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="1b162-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="1b162-113">Этот тип используется для предоставления параметров подключения OAuth1.</span><span class="sxs-lookup"><span data-stu-id="1b162-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="1b162-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="1b162-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="1b162-115">Этот тип используется для предоставления параметров подключения OAuth2 предоставить учетные данные клиента.</span><span class="sxs-lookup"><span data-stu-id="1b162-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b162-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b162-116">Properties</span></span>

| <span data-ttu-id="1b162-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b162-117">Property</span></span> | <span data-ttu-id="1b162-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1b162-118">Type</span></span> | <span data-ttu-id="1b162-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1b162-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1b162-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="1b162-120">**clientId**</span></span> | <span data-ttu-id="1b162-121">String</span><span class="sxs-lookup"><span data-stu-id="1b162-121">String</span></span> |  <span data-ttu-id="1b162-122">Идентификатор клиента, используемого для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="1b162-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="1b162-123">client_secret</span><span class="sxs-lookup"><span data-stu-id="1b162-123">**clientSecret**</span></span> | <span data-ttu-id="1b162-124">String</span><span class="sxs-lookup"><span data-stu-id="1b162-124">String</span></span> |  <span data-ttu-id="1b162-125">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="1b162-125">Client secret to authenticate the connection to the provider.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
