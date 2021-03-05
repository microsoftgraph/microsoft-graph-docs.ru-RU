---
title: тип ресурса certificateBasedAuthConfiguration
description: Представляет коллекцию органов сертификации.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8580851fe5f2c9266659b0bf26e85a9eca07185c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443904"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="34593-103">тип ресурса certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="34593-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34593-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34593-105">Проверка подлинности на основе сертификатов позволяет проверить подлинность в Azure Active Directory с клиентской сертификатом на устройстве Windows, Android или iOS при подключении учетной записи Exchange Online к:</span><span class="sxs-lookup"><span data-stu-id="34593-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="34593-106">Мобильные приложения Майкрософт, такие как Outlook и Word</span><span class="sxs-lookup"><span data-stu-id="34593-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="34593-107">Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="34593-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="34593-108">Настройка этой функции исключает необходимость ввода имени пользователя и сочетания паролей в определенные почтовые и Microsoft Office приложения на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="34593-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="34593-109">Конфигурация проверки подлинности на основе сертификатов предоставляется через коллекцию органов сертификации.</span><span class="sxs-lookup"><span data-stu-id="34593-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="34593-110">Органы сертификации используются для создания цепочки доверенных сертификатов, которая позволяет клиентам быть аутентификацией в Azure Active Directory с помощью клиентского сертификата.</span><span class="sxs-lookup"><span data-stu-id="34593-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="34593-111">Узнайте больше о проверке подлинности на основе [сертификатов в Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)</span><span class="sxs-lookup"><span data-stu-id="34593-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="34593-112">Методы</span><span class="sxs-lookup"><span data-stu-id="34593-112">Methods</span></span>

| <span data-ttu-id="34593-113">Метод</span><span class="sxs-lookup"><span data-stu-id="34593-113">Method</span></span>       | <span data-ttu-id="34593-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34593-114">Return Type</span></span> | <span data-ttu-id="34593-115">Описание</span><span class="sxs-lookup"><span data-stu-id="34593-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="34593-116">List certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="34593-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="34593-118">Список свойств коллекции **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="34593-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="34593-119">Создание certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-119">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="34593-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="34593-121">Создайте новый **объект certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="34593-121">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="34593-122">Получить certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-122">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="34593-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="34593-124">Ознакомьтесь с свойствами **объекта certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="34593-124">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="34593-125">Удаление certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="34593-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="34593-126">Нет</span><span class="sxs-lookup"><span data-stu-id="34593-126">None</span></span> | <span data-ttu-id="34593-127">Удаление **объекта certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="34593-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="34593-128">Обновление **certificateBasedAuthConfiguration** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34593-128">Updating **certificateBasedAuthConfiguration** is not supported.</span></span> <span data-ttu-id="34593-129">Чтобы изменить **certificateBasedAuthConfiguration,** сначала удалите, а затем создайте новый **сертификатBasedAuthConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="34593-129">To change a **certificateBasedAuthConfiguration**, first delete and then create a new **certificateBasedAuthConfiguration**.</span></span>

## <a name="properties"></a><span data-ttu-id="34593-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="34593-130">Properties</span></span>

| <span data-ttu-id="34593-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="34593-131">Property</span></span>     | <span data-ttu-id="34593-132">Тип</span><span class="sxs-lookup"><span data-stu-id="34593-132">Type</span></span>        | <span data-ttu-id="34593-133">Описание</span><span class="sxs-lookup"><span data-stu-id="34593-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34593-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="34593-134">certificateAuthorities</span></span>|<span data-ttu-id="34593-135">[коллекция certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="34593-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="34593-136">Коллекция органов сертификации, создав цепочку надежных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="34593-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="34593-137">id</span><span class="sxs-lookup"><span data-stu-id="34593-137">id</span></span>|<span data-ttu-id="34593-138">String</span><span class="sxs-lookup"><span data-stu-id="34593-138">String</span></span>|<span data-ttu-id="34593-139">Уникальный идентификатор конфигурации auth на основе сертификата.</span><span class="sxs-lookup"><span data-stu-id="34593-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="34593-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34593-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34593-141">Связи</span><span class="sxs-lookup"><span data-stu-id="34593-141">Relationships</span></span>

<span data-ttu-id="34593-142">Нет,</span><span class="sxs-lookup"><span data-stu-id="34593-142">None,</span></span>

## <a name="json-representation"></a><span data-ttu-id="34593-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34593-143">JSON representation</span></span>

<span data-ttu-id="34593-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34593-144">The following is a JSON representation of the resource.</span></span>

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
