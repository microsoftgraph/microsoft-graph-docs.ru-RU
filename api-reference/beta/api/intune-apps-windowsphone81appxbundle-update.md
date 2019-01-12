---
title: Обновление windowsPhone81AppXBundle
description: Обновление свойства объекта windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2902e95fc8b92a33f2b7e9597e8d96123e8eaef3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949096"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="6fa71-103">Обновление windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="6fa71-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="6fa71-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6fa71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fa71-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fa71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fa71-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6fa71-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fa71-107">Обновление свойства объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="6fa71-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fa71-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6fa71-108">Prerequisites</span></span>
<span data-ttu-id="6fa71-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fa71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fa71-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fa71-111">Permission type</span></span>|<span data-ttu-id="6fa71-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fa71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fa71-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fa71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fa71-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa71-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6fa71-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fa71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fa71-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fa71-116">Not supported.</span></span>|
|<span data-ttu-id="6fa71-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fa71-117">Application</span></span>|<span data-ttu-id="6fa71-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fa71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fa71-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fa71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6fa71-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fa71-120">Request headers</span></span>
|<span data-ttu-id="6fa71-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fa71-121">Header</span></span>|<span data-ttu-id="6fa71-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6fa71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fa71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fa71-123">Authorization</span></span>|<span data-ttu-id="6fa71-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6fa71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fa71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6fa71-125">Accept</span></span>|<span data-ttu-id="6fa71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa71-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6fa71-127">Request body</span></span>
<span data-ttu-id="6fa71-128">В тексте запроса укажите представление JSON для объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="6fa71-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="6fa71-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="6fa71-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fa71-130">Property</span></span>|<span data-ttu-id="6fa71-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6fa71-131">Type</span></span>|<span data-ttu-id="6fa71-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6fa71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa71-133">id</span><span class="sxs-lookup"><span data-stu-id="6fa71-133">id</span></span>|<span data-ttu-id="6fa71-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6fa71-134">String</span></span>|<span data-ttu-id="6fa71-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6fa71-135">Key of the entity.</span></span> <span data-ttu-id="6fa71-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6fa71-137">displayName</span></span>|<span data-ttu-id="6fa71-138">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-138">String</span></span>|<span data-ttu-id="6fa71-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="6fa71-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6fa71-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-141">описание</span><span class="sxs-lookup"><span data-stu-id="6fa71-141">description</span></span>|<span data-ttu-id="6fa71-142">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-142">String</span></span>|<span data-ttu-id="6fa71-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-143">The description of the app.</span></span> <span data-ttu-id="6fa71-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-145">publisher</span><span class="sxs-lookup"><span data-stu-id="6fa71-145">publisher</span></span>|<span data-ttu-id="6fa71-146">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-146">String</span></span>|<span data-ttu-id="6fa71-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-147">The publisher of the app.</span></span> <span data-ttu-id="6fa71-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6fa71-149">largeIcon</span></span>|[<span data-ttu-id="6fa71-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6fa71-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6fa71-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="6fa71-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6fa71-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa71-153">createdDateTime</span></span>|<span data-ttu-id="6fa71-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa71-154">DateTimeOffset</span></span>|<span data-ttu-id="6fa71-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-155">The date and time the app was created.</span></span> <span data-ttu-id="6fa71-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa71-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6fa71-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa71-158">DateTimeOffset</span></span>|<span data-ttu-id="6fa71-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6fa71-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6fa71-161">isFeatured</span></span>|<span data-ttu-id="6fa71-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fa71-162">Boolean</span></span>|<span data-ttu-id="6fa71-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6fa71-164">privacyInformationUrl</span></span>|<span data-ttu-id="6fa71-165">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-165">String</span></span>|<span data-ttu-id="6fa71-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6fa71-166">The privacy statement Url.</span></span> <span data-ttu-id="6fa71-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6fa71-168">informationUrl</span></span>|<span data-ttu-id="6fa71-169">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-169">String</span></span>|<span data-ttu-id="6fa71-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6fa71-170">The more information Url.</span></span> <span data-ttu-id="6fa71-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-172">owner</span><span class="sxs-lookup"><span data-stu-id="6fa71-172">owner</span></span>|<span data-ttu-id="6fa71-173">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-173">String</span></span>|<span data-ttu-id="6fa71-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-174">The owner of the app.</span></span> <span data-ttu-id="6fa71-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-176">developer</span><span class="sxs-lookup"><span data-stu-id="6fa71-176">developer</span></span>|<span data-ttu-id="6fa71-177">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-177">String</span></span>|<span data-ttu-id="6fa71-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-178">The developer of the app.</span></span> <span data-ttu-id="6fa71-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-180">notes</span><span class="sxs-lookup"><span data-stu-id="6fa71-180">notes</span></span>|<span data-ttu-id="6fa71-181">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-181">String</span></span>|<span data-ttu-id="6fa71-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="6fa71-182">Notes for the app.</span></span> <span data-ttu-id="6fa71-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6fa71-184">uploadState</span></span>|<span data-ttu-id="6fa71-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6fa71-185">Int32</span></span>|<span data-ttu-id="6fa71-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="6fa71-186">The upload state.</span></span> <span data-ttu-id="6fa71-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6fa71-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="6fa71-188">publishingState</span></span>|[<span data-ttu-id="6fa71-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6fa71-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6fa71-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-190">The publishing state for the app.</span></span> <span data-ttu-id="6fa71-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="6fa71-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6fa71-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6fa71-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6fa71-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6fa71-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6fa71-194">committedContentVersion</span></span>|<span data-ttu-id="6fa71-195">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-195">String</span></span>|<span data-ttu-id="6fa71-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="6fa71-196">The internal committed content version.</span></span> <span data-ttu-id="6fa71-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6fa71-198">fileName</span><span class="sxs-lookup"><span data-stu-id="6fa71-198">fileName</span></span>|<span data-ttu-id="6fa71-199">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-199">String</span></span>|<span data-ttu-id="6fa71-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-200">The name of the main Lob application file.</span></span> <span data-ttu-id="6fa71-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6fa71-202">size</span><span class="sxs-lookup"><span data-stu-id="6fa71-202">size</span></span>|<span data-ttu-id="6fa71-203">Int64</span><span class="sxs-lookup"><span data-stu-id="6fa71-203">Int64</span></span>|<span data-ttu-id="6fa71-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="6fa71-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="6fa71-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6fa71-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="6fa71-206">applicableArchitectures</span></span>|[<span data-ttu-id="6fa71-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="6fa71-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="6fa71-208">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="6fa71-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="6fa71-209">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="6fa71-209">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="6fa71-210">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="6fa71-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="6fa71-211">identityName</span><span class="sxs-lookup"><span data-stu-id="6fa71-211">identityName</span></span>|<span data-ttu-id="6fa71-212">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-212">String</span></span>|<span data-ttu-id="6fa71-213">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-213">The Identity Name.</span></span> <span data-ttu-id="6fa71-214">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6fa71-214">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6fa71-215">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="6fa71-215">identityPublisherHash</span></span>|<span data-ttu-id="6fa71-216">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-216">String</span></span>|<span data-ttu-id="6fa71-217">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6fa71-217">The Identity Publisher Hash.</span></span> <span data-ttu-id="6fa71-218">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6fa71-218">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6fa71-219">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6fa71-219">identityResourceIdentifier</span></span>|<span data-ttu-id="6fa71-220">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-220">String</span></span>|<span data-ttu-id="6fa71-221">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="6fa71-221">The Identity Resource Identifier.</span></span> <span data-ttu-id="6fa71-222">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6fa71-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6fa71-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6fa71-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6fa71-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6fa71-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="6fa71-225">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6fa71-225">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="6fa71-226">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6fa71-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6fa71-227">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="6fa71-227">phoneProductIdentifier</span></span>|<span data-ttu-id="6fa71-228">Строка</span><span class="sxs-lookup"><span data-stu-id="6fa71-228">String</span></span>|<span data-ttu-id="6fa71-229">Идентификатор продукта телефона.</span><span class="sxs-lookup"><span data-stu-id="6fa71-229">The Phone Product Identifier.</span></span> <span data-ttu-id="6fa71-230">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6fa71-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6fa71-231">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="6fa71-231">phonePublisherId</span></span>|<span data-ttu-id="6fa71-232">Строка</span><span class="sxs-lookup"><span data-stu-id="6fa71-232">String</span></span>|<span data-ttu-id="6fa71-233">Идентификатор издателя телефона наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6fa71-233">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6fa71-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6fa71-234">identityVersion</span></span>|<span data-ttu-id="6fa71-235">String</span><span class="sxs-lookup"><span data-stu-id="6fa71-235">String</span></span>|<span data-ttu-id="6fa71-236">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6fa71-236">The identity version.</span></span> <span data-ttu-id="6fa71-237">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6fa71-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6fa71-238">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="6fa71-238">appXPackageInformationList</span></span>|<span data-ttu-id="6fa71-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6fa71-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="6fa71-240">Список AppX сведения о пакете.</span><span class="sxs-lookup"><span data-stu-id="6fa71-240">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="6fa71-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fa71-241">Response</span></span>
<span data-ttu-id="6fa71-242">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6fa71-242">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fa71-243">Пример</span><span class="sxs-lookup"><span data-stu-id="6fa71-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fa71-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fa71-244">Request</span></span>
<span data-ttu-id="6fa71-245">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fa71-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2100

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
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6fa71-246">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fa71-246">Response</span></span>
<span data-ttu-id="6fa71-p127">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6fa71-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2271

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```





