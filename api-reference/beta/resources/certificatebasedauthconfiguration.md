---
title: тип ресурса certificateBasedAuthConfiguration
description: Представляет коллекцию органов сертификации.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1ff4eb3e7a235a27dc9d58b9b4bd631d0aeaed0f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443148"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="56523-103">тип ресурса certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="56523-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56523-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56523-105">Проверка подлинности на основе сертификатов позволяет проверить подлинность в Azure Active Directory с клиентской сертификатом на устройстве Windows, Android или iOS при подключении учетной записи Exchange Online к:</span><span class="sxs-lookup"><span data-stu-id="56523-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="56523-106">Мобильные приложения Майкрософт, такие как Outlook и Word</span><span class="sxs-lookup"><span data-stu-id="56523-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="56523-107">Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="56523-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="56523-108">Настройка этой функции исключает необходимость ввода имени пользователя и сочетания паролей в определенные почтовые и Microsoft Office приложения на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="56523-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="56523-109">Конфигурация проверки подлинности на основе сертификатов предоставляется через коллекцию органов сертификации.</span><span class="sxs-lookup"><span data-stu-id="56523-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="56523-110">Органы сертификации используются для создания цепочки доверенных сертификатов, которая позволяет клиентам быть аутентификацией в Azure Active Directory с помощью клиентского сертификата.</span><span class="sxs-lookup"><span data-stu-id="56523-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="56523-111">Узнайте больше о проверке подлинности на основе [сертификатов в Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)</span><span class="sxs-lookup"><span data-stu-id="56523-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="56523-112">Методы</span><span class="sxs-lookup"><span data-stu-id="56523-112">Methods</span></span>

| <span data-ttu-id="56523-113">Метод</span><span class="sxs-lookup"><span data-stu-id="56523-113">Method</span></span>       | <span data-ttu-id="56523-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="56523-114">Return Type</span></span> | <span data-ttu-id="56523-115">Описание</span><span class="sxs-lookup"><span data-stu-id="56523-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="56523-116">List certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="56523-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="56523-118">Список свойств коллекции **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="56523-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="56523-119">Получить certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-119">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="56523-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="56523-121">Ознакомьтесь с свойствами **объекта certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="56523-121">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="56523-122">Создание certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-122">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="56523-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="56523-124">Создайте новый **объект certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="56523-124">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="56523-125">Удаление certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="56523-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="56523-126">Нет</span><span class="sxs-lookup"><span data-stu-id="56523-126">None</span></span> | <span data-ttu-id="56523-127">Удаление **объекта certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="56523-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="56523-128">Обновление cerficateBasedAuthConfiguration не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56523-128">Updating cerficateBasedAuthConfiguration is not supported.</span></span> <span data-ttu-id="56523-129">Чтобы изменить cerficateBasedAuthConfiguration, сначала удалите, а затем создайте новую cerficateBasedAuthConfiguration.</span><span class="sxs-lookup"><span data-stu-id="56523-129">To change a cerficateBasedAuthConfiguration, first delete and then create a new cerficateBasedAuthConfiguration.</span></span>

## <a name="properties"></a><span data-ttu-id="56523-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="56523-130">Properties</span></span>

| <span data-ttu-id="56523-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="56523-131">Property</span></span>     | <span data-ttu-id="56523-132">Тип</span><span class="sxs-lookup"><span data-stu-id="56523-132">Type</span></span>        | <span data-ttu-id="56523-133">Описание</span><span class="sxs-lookup"><span data-stu-id="56523-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56523-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="56523-134">certificateAuthorities</span></span>|<span data-ttu-id="56523-135">[коллекция certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="56523-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="56523-136">Коллекция органов сертификации, создав цепочку надежных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="56523-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="56523-137">id</span><span class="sxs-lookup"><span data-stu-id="56523-137">id</span></span>|<span data-ttu-id="56523-138">String</span><span class="sxs-lookup"><span data-stu-id="56523-138">String</span></span>|<span data-ttu-id="56523-139">Уникальный идентификатор конфигурации auth на основе сертификата.</span><span class="sxs-lookup"><span data-stu-id="56523-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="56523-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="56523-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56523-141">Связи</span><span class="sxs-lookup"><span data-stu-id="56523-141">Relationships</span></span>

<span data-ttu-id="56523-142">Нет</span><span class="sxs-lookup"><span data-stu-id="56523-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56523-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56523-143">JSON representation</span></span>

<span data-ttu-id="56523-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56523-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
