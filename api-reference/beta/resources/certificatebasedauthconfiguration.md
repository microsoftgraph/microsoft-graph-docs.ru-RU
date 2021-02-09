---
title: Тип ресурса certificateBasedAuthConfiguration
description: Представляет коллекцию сертификатов.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b37022852407951fb850b8e82508cfff1973247f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161154"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="fb27c-103">Тип ресурса certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="fb27c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb27c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb27c-105">Проверка подлинности на основе сертификатов позволяет azure Active Directory проверить подлинность с помощью сертификата клиента на устройстве с Windows, Android или iOS при подключении учетной записи Exchange Online к:</span><span class="sxs-lookup"><span data-stu-id="fb27c-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="fb27c-106">Мобильные приложения Майкрософт, такие как Outlook и Word</span><span class="sxs-lookup"><span data-stu-id="fb27c-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="fb27c-107">Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="fb27c-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="fb27c-108">Настройка этой функции устраняет необходимость ввода имени пользователя и пароля в определенных почтовых Microsoft Office приложениях на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="fb27c-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="fb27c-109">Конфигурация проверки подлинности на основе сертификатов предоставляется с помощью коллекции сертификатных органов.</span><span class="sxs-lookup"><span data-stu-id="fb27c-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="fb27c-110">Эти органы используются для создания надежной цепочки сертификатов, которая позволяет клиентам аутентификацию с помощью Azure Active Directory с помощью сертификата клиента.</span><span class="sxs-lookup"><span data-stu-id="fb27c-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="fb27c-111">Узнайте больше о проверке подлинности на [основе сертификатов в Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)</span><span class="sxs-lookup"><span data-stu-id="fb27c-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="fb27c-112">Методы</span><span class="sxs-lookup"><span data-stu-id="fb27c-112">Methods</span></span>

| <span data-ttu-id="fb27c-113">Метод</span><span class="sxs-lookup"><span data-stu-id="fb27c-113">Method</span></span>       | <span data-ttu-id="fb27c-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb27c-114">Return Type</span></span> | <span data-ttu-id="fb27c-115">Описание</span><span class="sxs-lookup"><span data-stu-id="fb27c-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fb27c-116">Список certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="fb27c-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="fb27c-118">Список свойств коллекции **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="fb27c-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="fb27c-119">Get certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-119">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="fb27c-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="fb27c-121">Чтение свойств объекта **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="fb27c-121">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="fb27c-122">Создание certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-122">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="fb27c-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="fb27c-124">Создание объекта **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="fb27c-124">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="fb27c-125">Удаление certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb27c-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="fb27c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="fb27c-126">None</span></span> | <span data-ttu-id="fb27c-127">Удаление объекта **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="fb27c-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="fb27c-128">Обновление cerficateBasedAuthConfiguration не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb27c-128">Updating cerficateBasedAuthConfiguration is not supported.</span></span> <span data-ttu-id="fb27c-129">Чтобы изменить cerficateBasedAuthConfiguration, сначала удалите, а затем создайте новый cerficateBasedAuthConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb27c-129">To change a cerficateBasedAuthConfiguration, first delete and then create a new cerficateBasedAuthConfiguration.</span></span>

## <a name="properties"></a><span data-ttu-id="fb27c-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb27c-130">Properties</span></span>

| <span data-ttu-id="fb27c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb27c-131">Property</span></span>     | <span data-ttu-id="fb27c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fb27c-132">Type</span></span>        | <span data-ttu-id="fb27c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fb27c-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb27c-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="fb27c-134">certificateAuthorities</span></span>|<span data-ttu-id="fb27c-135">[Коллекция certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="fb27c-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="fb27c-136">Коллекция органов сертификации, которые создают доверенного цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fb27c-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="fb27c-137">id</span><span class="sxs-lookup"><span data-stu-id="fb27c-137">id</span></span>|<span data-ttu-id="fb27c-138">String</span><span class="sxs-lookup"><span data-stu-id="fb27c-138">String</span></span>|<span data-ttu-id="fb27c-139">Уникальный идентификатор конфигурации auth на основе сертификата.</span><span class="sxs-lookup"><span data-stu-id="fb27c-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="fb27c-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb27c-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb27c-141">Связи</span><span class="sxs-lookup"><span data-stu-id="fb27c-141">Relationships</span></span>

<span data-ttu-id="fb27c-142">Нет</span><span class="sxs-lookup"><span data-stu-id="fb27c-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb27c-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb27c-143">JSON representation</span></span>

<span data-ttu-id="fb27c-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb27c-144">The following is a JSON representation of the resource.</span></span>

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