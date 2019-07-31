---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c82d912b13ca68dcdccd5ace0232ed65f92cd879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972492"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="101ce-104">Тип ресурса Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="101ce-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="101ce-105">Представляет параметры подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="101ce-105">Represents the provider connection settings.</span></span> <span data-ttu-id="101ce-106">Это позволяет системе узнать, как подключаться к API поставщика.</span><span class="sxs-lookup"><span data-stu-id="101ce-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="101ce-107">**Примечание:** Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="101ce-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="101ce-108">Ознакомьтесь со списками определенных типов параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="101ce-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="101ce-109">Производные типы</span><span class="sxs-lookup"><span data-stu-id="101ce-109">Derived types</span></span>
| <span data-ttu-id="101ce-110">Тип</span><span class="sxs-lookup"><span data-stu-id="101ce-110">Type</span></span> | <span data-ttu-id="101ce-111">Описание</span><span class="sxs-lookup"><span data-stu-id="101ce-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="101ce-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="101ce-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="101ce-113">Используйте этот тип для предоставления параметров подключения OAuth1.</span><span class="sxs-lookup"><span data-stu-id="101ce-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="101ce-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="101ce-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="101ce-115">Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="101ce-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="101ce-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="101ce-116">Properties</span></span>

| <span data-ttu-id="101ce-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="101ce-117">Property</span></span> | <span data-ttu-id="101ce-118">Тип</span><span class="sxs-lookup"><span data-stu-id="101ce-118">Type</span></span> | <span data-ttu-id="101ce-119">Описание</span><span class="sxs-lookup"><span data-stu-id="101ce-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="101ce-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="101ce-120">**clientId**</span></span> | <span data-ttu-id="101ce-121">String</span><span class="sxs-lookup"><span data-stu-id="101ce-121">String</span></span> |  <span data-ttu-id="101ce-122">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="101ce-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="101ce-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="101ce-123">**clientSecret**</span></span> | <span data-ttu-id="101ce-124">String</span><span class="sxs-lookup"><span data-stu-id="101ce-124">String</span></span> |  <span data-ttu-id="101ce-125">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="101ce-125">Client secret to authenticate the connection to the provider.</span></span> |
