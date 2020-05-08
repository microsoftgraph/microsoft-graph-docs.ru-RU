---
title: Тип ресурса Profile
description: Представляет свойства, которые являются описательными для пользователя и представлены в общедоступных людях в Microsoft 365 и службах и возможностях сторонних производителей с помощью Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2e378229e8b001070db274c812cdb307934717cf
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168570"
---
# <a name="profile-resource-type"></a><span data-ttu-id="c12c0-103">Тип ресурса Profile</span><span class="sxs-lookup"><span data-stu-id="c12c0-103">profile resource type</span></span>

<span data-ttu-id="c12c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c12c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c12c0-105">Представляет свойства, которые являются описательными для пользователя в клиенте, например юбилеев и действия по образованию.</span><span class="sxs-lookup"><span data-stu-id="c12c0-105">Represents properties that are descriptive of a user in a tenant, for example, anniversaries and education activities.</span></span> <span data-ttu-id="c12c0-106">Эти свойства отображаются в общедоступных людях в Microsoft 365 и сторонних службах и возможностях в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c12c0-106">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

<span data-ttu-id="c12c0-107">Программным способом эти свойства выражаются в виде [связей](#relationships) ресурса **профиля** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-107">Programmatically, these properties are expressed as [relationships](#relationships) of the **profile** resource.</span></span> <span data-ttu-id="c12c0-108">Чтобы получить одно из этих свойств навигации или создать экземпляр этих свойств для пользователя, используйте соответствующий метод GET или POST для этого свойства там, где это уместно.</span><span class="sxs-lookup"><span data-stu-id="c12c0-108">To get one of these navigation properties or create an instance of these properties for the user, use the corresponding GET or POST method on that property, where applicable.</span></span> <span data-ttu-id="c12c0-109">Ознакомьтесь с приведенными ниже [способами](#methods) .</span><span class="sxs-lookup"><span data-stu-id="c12c0-109">See the [methods](#methods) listed below.</span></span>

## <a name="methods"></a><span data-ttu-id="c12c0-110">Методы</span><span class="sxs-lookup"><span data-stu-id="c12c0-110">Methods</span></span>

| <span data-ttu-id="c12c0-111">Метод</span><span class="sxs-lookup"><span data-stu-id="c12c0-111">Method</span></span>                                                                     | <span data-ttu-id="c12c0-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c12c0-112">Return Type</span></span>                                                    | <span data-ttu-id="c12c0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c12c0-113">Description</span></span>                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [<span data-ttu-id="c12c0-114">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="c12c0-114">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="c12c0-115">profile</span><span class="sxs-lookup"><span data-stu-id="c12c0-115">profile</span></span>](profile.md)                                          | <span data-ttu-id="c12c0-116">Чтение свойств и связей объекта Profile.</span><span class="sxs-lookup"><span data-stu-id="c12c0-116">Read properties and relationships of the profile object.</span></span>                                         |
| [<span data-ttu-id="c12c0-117">Удаление профиля</span><span class="sxs-lookup"><span data-stu-id="c12c0-117">Delete profile</span></span>](../api/profile-delete.md)                                 | <span data-ttu-id="c12c0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c12c0-118">None</span></span>                                                           | <span data-ttu-id="c12c0-119">Удаление объекта **Profile** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-119">Delete a **profile** object.</span></span>                                                                 |
| [<span data-ttu-id="c12c0-120">Учетная запись списка</span><span class="sxs-lookup"><span data-stu-id="c12c0-120">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="c12c0-121">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-121">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="c12c0-122">Получение коллекции объектов **усераккаунтинформатион** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-122">Get a **userAccountInformation** object collection.</span></span>                                          |
| [<span data-ttu-id="c12c0-123">Создание Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="c12c0-123">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="c12c0-124">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="c12c0-124">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="c12c0-125">Создание нового **персонанниверсари** путем публикации в коллекции юбилеев.</span><span class="sxs-lookup"><span data-stu-id="c12c0-125">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>               |
| [<span data-ttu-id="c12c0-126">Список юбилеев</span><span class="sxs-lookup"><span data-stu-id="c12c0-126">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="c12c0-127">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-127">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="c12c0-128">Получение коллекции объектов **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-128">Get a **personAnniversary** object collection.</span></span>                                               |
| [<span data-ttu-id="c12c0-129">Создание Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="c12c0-129">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="c12c0-130">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="c12c0-130">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="c12c0-131">Создание нового **едукатионалактивити** путем отправки в коллекцию **едукатионалактивитиес** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-131">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="c12c0-132">Список Едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="c12c0-132">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="c12c0-133">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-133">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="c12c0-134">Получение коллекции объектов **едукатионалактивити** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-134">Get an **educationalActivity** object collection.</span></span>                                            |
| [<span data-ttu-id="c12c0-135">Создание Итемемаил</span><span class="sxs-lookup"><span data-stu-id="c12c0-135">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="c12c0-136">итемемаил</span><span class="sxs-lookup"><span data-stu-id="c12c0-136">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="c12c0-137">Создание нового **итемемаил** путем отправки в коллекцию сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c12c0-137">Create a new **itemEmail** by posting to the emails collection.</span></span>                              |
| [<span data-ttu-id="c12c0-138">Список сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="c12c0-138">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="c12c0-139">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-139">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="c12c0-140">Получение коллекции объектов **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-140">Get an **itemEmail** object collection.</span></span>                                                      |
| [<span data-ttu-id="c12c0-141">Создание Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="c12c0-141">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="c12c0-142">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="c12c0-142">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="c12c0-143">Создание нового **персонинтерест** путем отправки в коллекцию интересов.</span><span class="sxs-lookup"><span data-stu-id="c12c0-143">Create a new **personInterest** by posting to the interests collection.</span></span>                      |
| [<span data-ttu-id="c12c0-144">Список интересов</span><span class="sxs-lookup"><span data-stu-id="c12c0-144">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="c12c0-145">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-145">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="c12c0-146">Получение коллекции объектов **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-146">Get a **personInterest** object collection.</span></span>                                                  |
| [<span data-ttu-id="c12c0-147">Создание ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c12c0-147">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="c12c0-148">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c12c0-148">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="c12c0-149">Создание нового **лангуажепрофиЦиенци** путем публикации в коллекции Languages.</span><span class="sxs-lookup"><span data-stu-id="c12c0-149">Create a new **languageProficiency** by posting to the languages collection.</span></span>                 |
| [<span data-ttu-id="c12c0-150">Список языков</span><span class="sxs-lookup"><span data-stu-id="c12c0-150">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="c12c0-151">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-151">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="c12c0-152">Получение коллекции объектов **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-152">Get a **languageProficiency** object collection.</span></span>                                             |
| [<span data-ttu-id="c12c0-153">Список имен</span><span class="sxs-lookup"><span data-stu-id="c12c0-153">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="c12c0-154">Коллекция [PersonName](personname.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-154">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="c12c0-155">Получение коллекции объектов **PersonName** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-155">Get a **personName** object collection.</span></span>                                                      |
| [<span data-ttu-id="c12c0-156">Создание personName</span><span class="sxs-lookup"><span data-stu-id="c12c0-156">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="c12c0-157">personName</span><span class="sxs-lookup"><span data-stu-id="c12c0-157">personName</span></span>](personName.md)                                    | <span data-ttu-id="c12c0-158">Создайте новый объект **PersonName** , отправив его в коллекцию Names.</span><span class="sxs-lookup"><span data-stu-id="c12c0-158">Create a new **personName** object by posting to the names collection.</span></span>                       |
| [<span data-ttu-id="c12c0-159">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="c12c0-159">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="c12c0-160">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-160">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="c12c0-161">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-161">Get a **personWebsite** object collection.</span></span>                                                   |
| [<span data-ttu-id="c12c0-162">Создание Итемфоне</span><span class="sxs-lookup"><span data-stu-id="c12c0-162">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="c12c0-163">итемфоне</span><span class="sxs-lookup"><span data-stu-id="c12c0-163">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="c12c0-164">Создание нового Итемфоне путем публикации в коллекции phones.</span><span class="sxs-lookup"><span data-stu-id="c12c0-164">Create a new itemPhone by posting to the phones collection.</span></span>                                  |
| [<span data-ttu-id="c12c0-165">Перечисление телефонов</span><span class="sxs-lookup"><span data-stu-id="c12c0-165">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="c12c0-166">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-166">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="c12c0-167">Получение коллекции объектов **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-167">Get a **itemPhone** object collection.</span></span>                                                       |
| [<span data-ttu-id="c12c0-168">Создание Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="c12c0-168">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="c12c0-169">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="c12c0-169">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="c12c0-170">Создание нового Воркпоситион путем отправки в коллекцию Positions.</span><span class="sxs-lookup"><span data-stu-id="c12c0-170">Create a new workPosition by posting to the positions collection.</span></span>                            |
| [<span data-ttu-id="c12c0-171">Позиции списка</span><span class="sxs-lookup"><span data-stu-id="c12c0-171">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="c12c0-172">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-172">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="c12c0-173">Получение коллекции объектов **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-173">Get a **workPosition** object collection.</span></span>                                                    |
| [<span data-ttu-id="c12c0-174">Создание ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="c12c0-174">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="c12c0-175">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="c12c0-175">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="c12c0-176">Создание нового **прожектпартиЦипатион** путем публикации в коллекции проектов.</span><span class="sxs-lookup"><span data-stu-id="c12c0-176">Create a new **projectParticipation** by posting to the projects collection.</span></span>                 |
| [<span data-ttu-id="c12c0-177">Список проектов</span><span class="sxs-lookup"><span data-stu-id="c12c0-177">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="c12c0-178">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-178">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="c12c0-179">Получение коллекции объектов **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-179">Get a **projectParticipation** object collection.</span></span>                                            |
| [<span data-ttu-id="c12c0-180">Создание СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c12c0-180">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="c12c0-181">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="c12c0-181">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="c12c0-182">Создание нового **скиллпрофиЦиенци** путем публикации в коллекции навыков.</span><span class="sxs-lookup"><span data-stu-id="c12c0-182">Create a new **skillProficiency** by posting to the skills collection.</span></span>                       |
| [<span data-ttu-id="c12c0-183">Список навыков</span><span class="sxs-lookup"><span data-stu-id="c12c0-183">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="c12c0-184">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-184">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="c12c0-185">Получение коллекции объектов **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-185">Get a **skillProficiency** object collection.</span></span>                                                |
| [<span data-ttu-id="c12c0-186">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="c12c0-186">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="c12c0-187">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="c12c0-187">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="c12c0-188">Создайте новую **учетную запись** , разместив ее в коллекции учетных записей.</span><span class="sxs-lookup"><span data-stu-id="c12c0-188">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                        |
| [<span data-ttu-id="c12c0-189">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="c12c0-189">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="c12c0-190">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-190">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="c12c0-191">Получение коллекции объектов **учетных записей** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-191">Get a **webAccount** object collection.</span></span>                                                      |
| [<span data-ttu-id="c12c0-192">Создание Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="c12c0-192">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="c12c0-193">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="c12c0-193">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="c12c0-194">Создание нового **персонвебсите** путем публикации в семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="c12c0-194">Create a new **personWebsite** by posting to the websites collection.</span></span>                        |
| [<span data-ttu-id="c12c0-195">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="c12c0-195">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="c12c0-196">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-196">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="c12c0-197">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="c12c0-197">Get a **personWebsite** object collection.</span></span>                                                   |

## <a name="properties"></a><span data-ttu-id="c12c0-198">Свойства</span><span class="sxs-lookup"><span data-stu-id="c12c0-198">Properties</span></span>

| <span data-ttu-id="c12c0-199">Свойство</span><span class="sxs-lookup"><span data-stu-id="c12c0-199">Property</span></span>     | <span data-ttu-id="c12c0-200">Тип</span><span class="sxs-lookup"><span data-stu-id="c12c0-200">Type</span></span>        | <span data-ttu-id="c12c0-201">Описание</span><span class="sxs-lookup"><span data-stu-id="c12c0-201">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c12c0-202">id</span><span class="sxs-lookup"><span data-stu-id="c12c0-202">id</span></span>            |<span data-ttu-id="c12c0-203">String</span><span class="sxs-lookup"><span data-stu-id="c12c0-203">String</span></span>       | <span data-ttu-id="c12c0-204">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-204">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="c12c0-205">Отношения</span><span class="sxs-lookup"><span data-stu-id="c12c0-205">Relationships</span></span>

| <span data-ttu-id="c12c0-206">Связь</span><span class="sxs-lookup"><span data-stu-id="c12c0-206">Relationship</span></span>          | <span data-ttu-id="c12c0-207">Тип</span><span class="sxs-lookup"><span data-stu-id="c12c0-207">Type</span></span>                                                         | <span data-ttu-id="c12c0-208">Описание</span><span class="sxs-lookup"><span data-stu-id="c12c0-208">Description</span></span>                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="c12c0-209">финансового</span><span class="sxs-lookup"><span data-stu-id="c12c0-209">account</span></span>                |<span data-ttu-id="c12c0-210">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-210">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="c12c0-211">Представляет сведения, специально связанные с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="c12c0-211">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="c12c0-212">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-212">Read-only.</span></span> <span data-ttu-id="c12c0-213">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-213">Nullable.</span></span>                                                             |
|<span data-ttu-id="c12c0-214">годовщины</span><span class="sxs-lookup"><span data-stu-id="c12c0-214">anniversaries</span></span>          |<span data-ttu-id="c12c0-215">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-215">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="c12c0-216">Представляет сведения о значимых датах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c12c0-216">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="c12c0-217">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-217">Read-only.</span></span> <span data-ttu-id="c12c0-218">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-218">Nullable.</span></span>                                                      |
|<span data-ttu-id="c12c0-219">едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="c12c0-219">educationalActivities</span></span>  |<span data-ttu-id="c12c0-220">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-220">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="c12c0-221">Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям.</span><span class="sxs-lookup"><span data-stu-id="c12c0-221">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="c12c0-222">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-222">Read-only.</span></span> <span data-ttu-id="c12c0-223">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-223">Nullable.</span></span>|
|<span data-ttu-id="c12c0-224">письма</span><span class="sxs-lookup"><span data-stu-id="c12c0-224">emails</span></span>                 |<span data-ttu-id="c12c0-225">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-225">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="c12c0-226">Представляет подробные сведения об адресах электронной почты, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c12c0-226">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="c12c0-227">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-227">Read-only.</span></span> <span data-ttu-id="c12c0-228">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-228">Nullable.</span></span>                                           |
|<span data-ttu-id="c12c0-229">interests;</span><span class="sxs-lookup"><span data-stu-id="c12c0-229">interests</span></span>              |<span data-ttu-id="c12c0-230">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-230">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="c12c0-231">Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c12c0-231">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="c12c0-232">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-232">Read-only.</span></span> <span data-ttu-id="c12c0-233">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-233">Nullable.</span></span>                |
|<span data-ttu-id="c12c0-234">Языки</span><span class="sxs-lookup"><span data-stu-id="c12c0-234">languages</span></span>              |<span data-ttu-id="c12c0-235">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-235">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="c12c0-236">Представляет подробные сведения о языках, добавленных пользователем в свой профиль.</span><span class="sxs-lookup"><span data-stu-id="c12c0-236">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="c12c0-237">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-237">Read-only.</span></span> <span data-ttu-id="c12c0-238">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-238">Nullable.</span></span>                                   |
|<span data-ttu-id="c12c0-239">phones</span><span class="sxs-lookup"><span data-stu-id="c12c0-239">phones</span></span>                 |<span data-ttu-id="c12c0-240">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-240">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="c12c0-241">Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c12c0-241">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="c12c0-242">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-242">Read-only.</span></span> <span data-ttu-id="c12c0-243">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-243">Nullable.</span></span>                           |
|<span data-ttu-id="c12c0-244">расположен</span><span class="sxs-lookup"><span data-stu-id="c12c0-244">positions</span></span>              |<span data-ttu-id="c12c0-245">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-245">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="c12c0-246">Представляет подробные сведения о должностных единицах, связанных с профилем пользователя.</span><span class="sxs-lookup"><span data-stu-id="c12c0-246">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="c12c0-247">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-247">Read-only.</span></span> <span data-ttu-id="c12c0-248">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-248">Nullable.</span></span>                                    |
|<span data-ttu-id="c12c0-249">projects</span><span class="sxs-lookup"><span data-stu-id="c12c0-249">projects</span></span>               |<span data-ttu-id="c12c0-250">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-250">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="c12c0-251">Представляет подробные сведения о проектах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c12c0-251">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="c12c0-252">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-252">Read-only.</span></span> <span data-ttu-id="c12c0-253">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-253">Nullable.</span></span>                                                    |
|<span data-ttu-id="c12c0-254">skills.</span><span class="sxs-lookup"><span data-stu-id="c12c0-254">skills</span></span>                 |<span data-ttu-id="c12c0-255">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-255">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="c12c0-256">Представляет подробные сведения о навыках, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c12c0-256">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="c12c0-257">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-257">Read-only.</span></span> <span data-ttu-id="c12c0-258">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-258">Nullable.</span></span>                                  |
|<span data-ttu-id="c12c0-259">Учетные записи учетных записей</span><span class="sxs-lookup"><span data-stu-id="c12c0-259">webAccounts</span></span>            |<span data-ttu-id="c12c0-260">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-260">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="c12c0-261">Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой профиль пользователя.</span><span class="sxs-lookup"><span data-stu-id="c12c0-261">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="c12c0-262">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-262">Read-only.</span></span> <span data-ttu-id="c12c0-263">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-263">Nullable.</span></span>                               |
|<span data-ttu-id="c12c0-264">websites</span><span class="sxs-lookup"><span data-stu-id="c12c0-264">websites</span></span>               |<span data-ttu-id="c12c0-265">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="c12c0-265">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="c12c0-266">Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c12c0-266">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="c12c0-267">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c12c0-267">Read-only.</span></span> <span data-ttu-id="c12c0-268">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c12c0-268">Nullable.</span></span>                                |

## <a name="json-representation"></a><span data-ttu-id="c12c0-269">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c12c0-269">JSON representation</span></span>

<span data-ttu-id="c12c0-270">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c12c0-270">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```

<!--
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
-->


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
