---
title: Тип ресурса certificateBasedAuthConfiguration
description: Представляет коллекцию сертификатов.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fcc5f37cb55ad0cc5e9e76bf0fe7efb6c4ab517
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153482"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="4924a-103">Тип ресурса certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="4924a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4924a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4924a-105">Проверка подлинности на основе сертификатов позволяет azure Active Directory проверить подлинность с помощью сертификата клиента на устройстве с Windows, Android или iOS при подключении учетной записи Exchange Online к:</span><span class="sxs-lookup"><span data-stu-id="4924a-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="4924a-106">Мобильные приложения Майкрософт, такие как Outlook и Word</span><span class="sxs-lookup"><span data-stu-id="4924a-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="4924a-107">Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="4924a-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="4924a-108">Настройка этой функции устраняет необходимость ввода имени пользователя и пароля в определенных почтовых Microsoft Office приложениях на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="4924a-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="4924a-109">Конфигурация проверки подлинности на основе сертификатов предоставляется с помощью коллекции сертификатных органов.</span><span class="sxs-lookup"><span data-stu-id="4924a-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="4924a-110">Эти органы используются для создания надежной цепочки сертификатов, которая позволяет клиентам аутентификацию с помощью Azure Active Directory с помощью сертификата клиента.</span><span class="sxs-lookup"><span data-stu-id="4924a-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="4924a-111">Узнайте больше о проверке подлинности на [основе сертификатов в Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)</span><span class="sxs-lookup"><span data-stu-id="4924a-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="4924a-112">Методы</span><span class="sxs-lookup"><span data-stu-id="4924a-112">Methods</span></span>

| <span data-ttu-id="4924a-113">Метод</span><span class="sxs-lookup"><span data-stu-id="4924a-113">Method</span></span>       | <span data-ttu-id="4924a-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4924a-114">Return Type</span></span> | <span data-ttu-id="4924a-115">Описание</span><span class="sxs-lookup"><span data-stu-id="4924a-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4924a-116">Список certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="4924a-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="4924a-118">Список свойств коллекции **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="4924a-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="4924a-119">Создание certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-119">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="4924a-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="4924a-121">Создание объекта **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="4924a-121">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="4924a-122">Get certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-122">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="4924a-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="4924a-124">Чтение свойств объекта **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="4924a-124">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="4924a-125">Удаление certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="4924a-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="4924a-126">Нет</span><span class="sxs-lookup"><span data-stu-id="4924a-126">None</span></span> | <span data-ttu-id="4924a-127">Удаление объекта **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="4924a-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="4924a-128">Обновление **certificateBasedAuthConfiguration** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4924a-128">Updating **certificateBasedAuthConfiguration** is not supported.</span></span> <span data-ttu-id="4924a-129">Чтобы изменить **certificateBasedAuthConfiguration,** сначала удалите, а затем создайте **новый certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="4924a-129">To change a **certificateBasedAuthConfiguration**, first delete and then create a new **certificateBasedAuthConfiguration**.</span></span>

## <a name="properties"></a><span data-ttu-id="4924a-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="4924a-130">Properties</span></span>

| <span data-ttu-id="4924a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4924a-131">Property</span></span>     | <span data-ttu-id="4924a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4924a-132">Type</span></span>        | <span data-ttu-id="4924a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4924a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4924a-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="4924a-134">certificateAuthorities</span></span>|<span data-ttu-id="4924a-135">[Коллекция certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="4924a-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="4924a-136">Коллекция органов сертификации, создав цепочку доверенных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4924a-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="4924a-137">id</span><span class="sxs-lookup"><span data-stu-id="4924a-137">id</span></span>|<span data-ttu-id="4924a-138">String</span><span class="sxs-lookup"><span data-stu-id="4924a-138">String</span></span>|<span data-ttu-id="4924a-139">Уникальный идентификатор конфигурации auth на основе сертификата.</span><span class="sxs-lookup"><span data-stu-id="4924a-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="4924a-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4924a-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4924a-141">Связи</span><span class="sxs-lookup"><span data-stu-id="4924a-141">Relationships</span></span>

<span data-ttu-id="4924a-142">Нет,</span><span class="sxs-lookup"><span data-stu-id="4924a-142">None,</span></span>

## <a name="json-representation"></a><span data-ttu-id="4924a-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4924a-143">JSON representation</span></span>

<span data-ttu-id="4924a-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4924a-144">The following is a JSON representation of the resource.</span></span>

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
