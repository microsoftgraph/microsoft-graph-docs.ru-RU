---
title: Обновление windowsPhone81AppX
description: Обновление свойства объекта windowsPhone81AppX.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 78c59cf0f2aaf76e735425aa5c553f75c1ea1eb0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939709"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="dfaee-103">Обновление windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="dfaee-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="dfaee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dfaee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfaee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfaee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfaee-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dfaee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfaee-107">Обновление свойства объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="dfaee-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dfaee-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dfaee-108">Prerequisites</span></span>
<span data-ttu-id="dfaee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfaee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfaee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfaee-111">Permission type</span></span>|<span data-ttu-id="dfaee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfaee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfaee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfaee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfaee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfaee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dfaee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfaee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfaee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfaee-116">Not supported.</span></span>|
|<span data-ttu-id="dfaee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfaee-117">Application</span></span>|<span data-ttu-id="dfaee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfaee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfaee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfaee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="dfaee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfaee-120">Request headers</span></span>
|<span data-ttu-id="dfaee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfaee-121">Header</span></span>|<span data-ttu-id="dfaee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dfaee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfaee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfaee-123">Authorization</span></span>|<span data-ttu-id="dfaee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dfaee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfaee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dfaee-125">Accept</span></span>|<span data-ttu-id="dfaee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfaee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfaee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfaee-127">Request body</span></span>
<span data-ttu-id="dfaee-128">В тексте запроса укажите представление JSON для объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="dfaee-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="dfaee-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="dfaee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfaee-130">Property</span></span>|<span data-ttu-id="dfaee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dfaee-131">Type</span></span>|<span data-ttu-id="dfaee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dfaee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfaee-133">id</span><span class="sxs-lookup"><span data-stu-id="dfaee-133">id</span></span>|<span data-ttu-id="dfaee-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dfaee-134">String</span></span>|<span data-ttu-id="dfaee-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dfaee-135">Key of the entity.</span></span> <span data-ttu-id="dfaee-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dfaee-137">displayName</span></span>|<span data-ttu-id="dfaee-138">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-138">String</span></span>|<span data-ttu-id="dfaee-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="dfaee-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dfaee-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-141">описание</span><span class="sxs-lookup"><span data-stu-id="dfaee-141">description</span></span>|<span data-ttu-id="dfaee-142">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-142">String</span></span>|<span data-ttu-id="dfaee-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-143">The description of the app.</span></span> <span data-ttu-id="dfaee-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-145">publisher</span><span class="sxs-lookup"><span data-stu-id="dfaee-145">publisher</span></span>|<span data-ttu-id="dfaee-146">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-146">String</span></span>|<span data-ttu-id="dfaee-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-147">The publisher of the app.</span></span> <span data-ttu-id="dfaee-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dfaee-149">largeIcon</span></span>|[<span data-ttu-id="dfaee-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dfaee-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dfaee-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="dfaee-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dfaee-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfaee-153">createdDateTime</span></span>|<span data-ttu-id="dfaee-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfaee-154">DateTimeOffset</span></span>|<span data-ttu-id="dfaee-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-155">The date and time the app was created.</span></span> <span data-ttu-id="dfaee-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfaee-157">lastModifiedDateTime</span></span>|<span data-ttu-id="dfaee-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfaee-158">DateTimeOffset</span></span>|<span data-ttu-id="dfaee-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-159">The date and time the app was last modified.</span></span> <span data-ttu-id="dfaee-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dfaee-161">isFeatured</span></span>|<span data-ttu-id="dfaee-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfaee-162">Boolean</span></span>|<span data-ttu-id="dfaee-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dfaee-164">privacyInformationUrl</span></span>|<span data-ttu-id="dfaee-165">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-165">String</span></span>|<span data-ttu-id="dfaee-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="dfaee-166">The privacy statement Url.</span></span> <span data-ttu-id="dfaee-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dfaee-168">informationUrl</span></span>|<span data-ttu-id="dfaee-169">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-169">String</span></span>|<span data-ttu-id="dfaee-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="dfaee-170">The more information Url.</span></span> <span data-ttu-id="dfaee-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-172">owner</span><span class="sxs-lookup"><span data-stu-id="dfaee-172">owner</span></span>|<span data-ttu-id="dfaee-173">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-173">String</span></span>|<span data-ttu-id="dfaee-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-174">The owner of the app.</span></span> <span data-ttu-id="dfaee-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-176">developer</span><span class="sxs-lookup"><span data-stu-id="dfaee-176">developer</span></span>|<span data-ttu-id="dfaee-177">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-177">String</span></span>|<span data-ttu-id="dfaee-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-178">The developer of the app.</span></span> <span data-ttu-id="dfaee-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-180">notes</span><span class="sxs-lookup"><span data-stu-id="dfaee-180">notes</span></span>|<span data-ttu-id="dfaee-181">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-181">String</span></span>|<span data-ttu-id="dfaee-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="dfaee-182">Notes for the app.</span></span> <span data-ttu-id="dfaee-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="dfaee-184">uploadState</span></span>|<span data-ttu-id="dfaee-185">Int32</span><span class="sxs-lookup"><span data-stu-id="dfaee-185">Int32</span></span>|<span data-ttu-id="dfaee-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="dfaee-186">The upload state.</span></span> <span data-ttu-id="dfaee-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dfaee-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="dfaee-188">publishingState</span></span>|[<span data-ttu-id="dfaee-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dfaee-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dfaee-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-190">The publishing state for the app.</span></span> <span data-ttu-id="dfaee-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="dfaee-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dfaee-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dfaee-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dfaee-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dfaee-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dfaee-194">committedContentVersion</span></span>|<span data-ttu-id="dfaee-195">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-195">String</span></span>|<span data-ttu-id="dfaee-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="dfaee-196">The internal committed content version.</span></span> <span data-ttu-id="dfaee-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dfaee-198">fileName</span><span class="sxs-lookup"><span data-stu-id="dfaee-198">fileName</span></span>|<span data-ttu-id="dfaee-199">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-199">String</span></span>|<span data-ttu-id="dfaee-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-200">The name of the main Lob application file.</span></span> <span data-ttu-id="dfaee-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dfaee-202">size</span><span class="sxs-lookup"><span data-stu-id="dfaee-202">size</span></span>|<span data-ttu-id="dfaee-203">Int64</span><span class="sxs-lookup"><span data-stu-id="dfaee-203">Int64</span></span>|<span data-ttu-id="dfaee-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="dfaee-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="dfaee-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dfaee-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dfaee-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="dfaee-206">applicableArchitectures</span></span>|[<span data-ttu-id="dfaee-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="dfaee-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="dfaee-208">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="dfaee-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="dfaee-209">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="dfaee-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="dfaee-210">identityName</span><span class="sxs-lookup"><span data-stu-id="dfaee-210">identityName</span></span>|<span data-ttu-id="dfaee-211">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-211">String</span></span>|<span data-ttu-id="dfaee-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-212">The Identity Name.</span></span>|
|<span data-ttu-id="dfaee-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="dfaee-213">identityPublisherHash</span></span>|<span data-ttu-id="dfaee-214">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-214">String</span></span>|<span data-ttu-id="dfaee-215">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="dfaee-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="dfaee-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="dfaee-216">identityResourceIdentifier</span></span>|<span data-ttu-id="dfaee-217">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-217">String</span></span>|<span data-ttu-id="dfaee-218">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="dfaee-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="dfaee-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dfaee-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dfaee-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dfaee-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="dfaee-221">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="dfaee-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="dfaee-222">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="dfaee-222">phoneProductIdentifier</span></span>|<span data-ttu-id="dfaee-223">Строка</span><span class="sxs-lookup"><span data-stu-id="dfaee-223">String</span></span>|<span data-ttu-id="dfaee-224">Идентификатор продукта телефона.</span><span class="sxs-lookup"><span data-stu-id="dfaee-224">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="dfaee-225">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="dfaee-225">phonePublisherId</span></span>|<span data-ttu-id="dfaee-226">Строка</span><span class="sxs-lookup"><span data-stu-id="dfaee-226">String</span></span>|<span data-ttu-id="dfaee-227">Publisher с идентификатором телефона.</span><span class="sxs-lookup"><span data-stu-id="dfaee-227">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="dfaee-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="dfaee-228">identityVersion</span></span>|<span data-ttu-id="dfaee-229">String</span><span class="sxs-lookup"><span data-stu-id="dfaee-229">String</span></span>|<span data-ttu-id="dfaee-230">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="dfaee-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="dfaee-231">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfaee-231">Response</span></span>
<span data-ttu-id="dfaee-232">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dfaee-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfaee-233">Пример</span><span class="sxs-lookup"><span data-stu-id="dfaee-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="dfaee-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfaee-234">Request</span></span>
<span data-ttu-id="dfaee-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfaee-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1362

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="dfaee-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfaee-236">Response</span></span>
<span data-ttu-id="dfaee-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dfaee-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1527

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```





