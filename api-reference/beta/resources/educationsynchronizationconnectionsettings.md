---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 449dc1c4265355d55e6d3ceb51fe86be9f84ac31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979565"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="34ea7-104">Тип ресурса Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="34ea7-104">educationSynchronizationConnectionSettings resource type</span></span>

<span data-ttu-id="34ea7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34ea7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34ea7-106">Представляет параметры подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="34ea7-106">Represents the provider connection settings.</span></span> <span data-ttu-id="34ea7-107">Это позволяет системе узнать, как подключаться к API поставщика.</span><span class="sxs-lookup"><span data-stu-id="34ea7-107">This allows the system to know how to connect to the provider APIs.</span></span>

> [!NOTE]
> <span data-ttu-id="34ea7-108">Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="34ea7-108">This complex type is abstract.</span></span> <span data-ttu-id="34ea7-109">Ознакомьтесь со списками определенных типов параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="34ea7-109">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="34ea7-110">Производные типы</span><span class="sxs-lookup"><span data-stu-id="34ea7-110">Derived types</span></span>

| <span data-ttu-id="34ea7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="34ea7-111">Type</span></span>                                                                                                                                      | <span data-ttu-id="34ea7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="34ea7-112">Description</span></span>                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [<span data-ttu-id="34ea7-113">educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="34ea7-113">educationSynchronizationOAuth1ConnectionSettings</span></span>](educationsynchronizationoauth1connectionsettings.md)                                   | <span data-ttu-id="34ea7-114">Используйте этот тип для предоставления параметров подключения OAuth1.</span><span class="sxs-lookup"><span data-stu-id="34ea7-114">Use this type to provide OAuth1 connection settings.</span></span>                          |
| [<span data-ttu-id="34ea7-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="34ea7-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="34ea7-116">Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="34ea7-116">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="34ea7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="34ea7-117">Properties</span></span>

| <span data-ttu-id="34ea7-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="34ea7-118">Property</span></span>     | <span data-ttu-id="34ea7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="34ea7-119">Type</span></span>   | <span data-ttu-id="34ea7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="34ea7-120">Description</span></span>                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="34ea7-121">clientId</span><span class="sxs-lookup"><span data-stu-id="34ea7-121">clientId</span></span>     | <span data-ttu-id="34ea7-122">String</span><span class="sxs-lookup"><span data-stu-id="34ea7-122">String</span></span> | <span data-ttu-id="34ea7-123">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="34ea7-123">Client ID used to connect to the provider.</span></span>                    |
| <span data-ttu-id="34ea7-124">clientSecret</span><span class="sxs-lookup"><span data-stu-id="34ea7-124">clientSecret</span></span> | <span data-ttu-id="34ea7-125">String</span><span class="sxs-lookup"><span data-stu-id="34ea7-125">String</span></span> | <span data-ttu-id="34ea7-126">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="34ea7-126">Client secret to authenticate the connection to the provider.</span></span> |


