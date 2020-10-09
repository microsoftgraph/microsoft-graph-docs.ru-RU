---
title: Тип ресурса Цертификатебаседаусконфигуратион
description: Представляет коллекцию центров сертификации.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6afa60a48522596754bb1991f2e9982d4a8ed8c
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401794"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="987a4-103">Тип ресурса Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="987a4-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="987a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="987a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="987a4-105">Проверка подлинности на основе сертификатов обеспечивает проверку подлинности Azure Active Directory с помощью сертификата клиента на устройстве Windows, Android или iOS при подключении учетной записи Exchange Online к:</span><span class="sxs-lookup"><span data-stu-id="987a4-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="987a4-106">Мобильные приложения Майкрософт, такие как Outlook и Word</span><span class="sxs-lookup"><span data-stu-id="987a4-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="987a4-107">Клиенты Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="987a4-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="987a4-108">Настройка этой функции исключает необходимость ввода имени пользователя и пароля в определенные приложения электронной почты и приложения Microsoft Office на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="987a4-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="987a4-109">Настройка проверки подлинности на основе сертификатов обеспечивается через коллекцию центров сертификации.</span><span class="sxs-lookup"><span data-stu-id="987a4-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="987a4-110">Центры сертификации используются для установки доверенной цепочки сертификатов, что позволяет клиентам выполнять проверку подлинности с помощью Azure Active Directory с помощью сертификата клиента.</span><span class="sxs-lookup"><span data-stu-id="987a4-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="987a4-111">Узнайте больше о [проверке подлинности на основе сертификатов в Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span><span class="sxs-lookup"><span data-stu-id="987a4-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="987a4-112">Методы</span><span class="sxs-lookup"><span data-stu-id="987a4-112">Methods</span></span>

| <span data-ttu-id="987a4-113">Метод</span><span class="sxs-lookup"><span data-stu-id="987a4-113">Method</span></span>       | <span data-ttu-id="987a4-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="987a4-114">Return Type</span></span> | <span data-ttu-id="987a4-115">Описание</span><span class="sxs-lookup"><span data-stu-id="987a4-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="987a4-116">Список Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="987a4-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="987a4-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="987a4-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="987a4-118">Перечисление свойств коллекции **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="987a4-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="987a4-119">Получение Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="987a4-119">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="987a4-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="987a4-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="987a4-121">Чтение свойств объекта **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="987a4-121">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="987a4-122">Создание Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="987a4-122">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="987a4-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="987a4-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="987a4-124">Создание нового объекта **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="987a4-124">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="987a4-125">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="987a4-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="987a4-126">Нет</span><span class="sxs-lookup"><span data-stu-id="987a4-126">None</span></span> | <span data-ttu-id="987a4-127">Удаление объекта **цертификатебаседаусконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="987a4-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="987a4-128">Обновление Церфикатебаседаусконфигуратион не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="987a4-128">Updating cerficateBasedAuthConfiguration is not supported.</span></span> <span data-ttu-id="987a4-129">Чтобы изменить Церфикатебаседаусконфигуратион, сначала удалите его, а затем создайте новый Церфикатебаседаусконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="987a4-129">To change a cerficateBasedAuthConfiguration, first delete and then create a new cerficateBasedAuthConfiguration.</span></span>

## <a name="properties"></a><span data-ttu-id="987a4-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="987a4-130">Properties</span></span>

| <span data-ttu-id="987a4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="987a4-131">Property</span></span>     | <span data-ttu-id="987a4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="987a4-132">Type</span></span>        | <span data-ttu-id="987a4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="987a4-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="987a4-134">цертификатеаусоритиес</span><span class="sxs-lookup"><span data-stu-id="987a4-134">certificateAuthorities</span></span>|<span data-ttu-id="987a4-135">Коллекция [цертификатеаусорити](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="987a4-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="987a4-136">Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="987a4-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="987a4-137">id</span><span class="sxs-lookup"><span data-stu-id="987a4-137">id</span></span>|<span data-ttu-id="987a4-138">String</span><span class="sxs-lookup"><span data-stu-id="987a4-138">String</span></span>|<span data-ttu-id="987a4-139">Уникальный идентификатор конфигурации проверки подлинности на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="987a4-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="987a4-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="987a4-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="987a4-141">Связи</span><span class="sxs-lookup"><span data-stu-id="987a4-141">Relationships</span></span>

<span data-ttu-id="987a4-142">Нет</span><span class="sxs-lookup"><span data-stu-id="987a4-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="987a4-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="987a4-143">JSON representation</span></span>

<span data-ttu-id="987a4-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="987a4-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "",
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