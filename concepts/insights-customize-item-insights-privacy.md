---
title: Настройка элемента конфиденциальности insights в Microsoft Graph
description: Обзор настройки аналитики элементов на уровне организации
author: simonhult
ms.localizationpriority: high
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: 7ce17257ac6d300b9006472261a913663d654d3f
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848638"
---
# <a name="customizing-item-insights-privacy-in-microsoft-graph-preview"></a>Настройка элемента конфиденциальности insights в Microsoft Graph (предварительный просмотр)

Аналитические выводы по элементам — это отношения, вычисленные корпорацией Майкрософт с помощью передовых методов машинного обучения. Когда пользователи совместно работают над документами, сайтами и списками SharePoint, чатами и каналами Teams, Майкрософт агрегирует эти действия в качестве сигналов. На основе этих сигналов корпорация Майкрософт генерирует рекомендации по контенту, ориентированному на пользователей, для пользователей в организации.

Аналитика элементов поможет пользователям быстро находить файлы, которые им важны, например в интерфейсе **Рекомендуемые** в Office.com и Delve. Пользователи могут обнаружить в области **Обзор** Outlook Mobile потенциально полезное содержимое, к которому у них есть доступ, но которое они, возможно, раньше не видели. Н?а основе персонализированных данных, таких как **Последние файлы** в карточке пользователя в Bing и **Последние** в приложениях Microsoft 365, пользователи могут с легкостью находить файлы, над которыми недавно работали.

Аналитические выводы по элементам отражают только содержимое, к которому у пользователей есть доступ. Пользователю не может быть рекомендовано содержимое, к которому у него нет доступа.

> **Примечание** Эта статья не касается других аналитических функций в Microsoft 365, таких как Viva Аналитика, Надстройка "Аналитика" для Outlook, функция WorkWith, MyAnalytics и информационная панель Insights.


## <a name="item-insights-privacy"></a>Конфиденциальность аналитики элементов 

Параметры конфиденциальности элемента insights позволяют настраивать видимость информации, получаемой из Microsoft Graph, между пользователями и другими элементами (например, документами и сайтами) в Microsoft 365. Вы можете отключить приложение Delve с помощью уже существующих элементов управления, но также использовать в дальнейшем другие полезные возможности, связанные с insights.

В этой статье описывается настройка конфиденциальности аналитики элементов в организации. Сведения о настройке аналитики элементов для пользователя см. в ресурсе [userInsightsSettings](/graph/api/resources/userinsightssettings?view=graph-rest-beta&preserve-view=true). Эти параметры для пользователя доступны с помощью свойства навигации с именем **itemInsights** в ресурсе [userSettings](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true).

## <a name="background"></a>Общие сведения
На момент первого выпуска в 2014 году, Office Graph был внутренней службой для Delve. Был представлен набор элементов управления конфиденциальностью как в Office Graph, так и в пользовательском интерфейсе Delve. С тех пор Office Graph развивался и стал более независимой и мощной частью интерфейса Microsoft 365, а также Microsoft Graph. Чтобы предложить связанную схему Microsoft Graph, компания Майкрософт представила элемент [itemInsights](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true), который наследует все свойства ранее существовавшего ресурса [officeGraphInsights](/graph/api/resources/officegraphinsights?view=graph-rest-beta&preserve-view=true), и сохранила **officeGraphInsights** для обеспечения обратной совместимости. Введение **itemInsights** также разделяет историю конфиденциальности на две независимые части.  

Хотя существующие приложения могут продолжать использовать **officeGraphInsights**, их следует обновить до **itemInsights**, чтобы обеспечить гибкую настройку элементов в Office Graph и Delve.

## <a name="how-to-customize-item-insights"></a>Как настроить элемент insights?

С помощью параметров аналитики элементов администраторы получают возможность гибко использовать инструменты Azure AD. Администраторы могут отключать аналитику элементов для всей организации или только для участников указанной группы Azure AD. Настройку аналитики элементов можно проводить через центр администрирования Microsoft 365 или использовать для этой цели пакет SDK PowerShell SDK или REST API Microsoft Graph с соответствующими разрешениями. Помните, что требуется _роль глобального администратора_. 

В следующем разделе описывается использование Центра администрирования, а за ним следует раздел о командлетах PowerShell. Если вы используете API REST, пропустите следующие два раздела и сразу перейдите к разделу [Настройка аналитики элементов с помощью REST API](#configure-item-insights-using-rest-api). Дополнительные сведения см. в описании операций REST [read](/graph/api/organizationsettings-list-iteminsights?view=graph-rest-beta&preserve-view=true) или [update](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true).

### <a name="how-to-configure-item-insights-settings-via-microsoft-admin-center"></a>Как настроить параметры аналитики элементов через Центр администрирования Майкрософт?
Администратор с _ролью глобального администратора_ может настраивать параметры конфиденциальности аналитики элементов с помощью переключателей. Для этого в Центре администрирования Microsoft 365 разверните раздел **Параметры**, выберите **Поиск и аналитика**, а затем в пункте **Аналитика элементов** выберите **Изменить параметры**.
![изображение](https://user-images.githubusercontent.com/54312959/117024482-b39eca00-ad02-11eb-9a11-e6a01039822e.png)


### <a name="how-to-configure-item-insights-settings-via-powershell"></a>Как настроить параметры аналитики элементов с помощью PowerShell?
Убедитесь, что выполнены следующие дополнительные предварительные требования. После этого используйте пакет [SDK PowerShell Microsoft Graph](/powershell/microsoftgraph/installation.md), чтобы настроить аналитику элементов для всей организации или для определенных групп.

#### <a name="additional-prerequisites"></a>Дополнительные предварительные требования
* **Модуль PowerShell** — установите [модуль версии 0.9.1 или более поздней](https://www.powershellgallery.com/packages/Microsoft.Graph).
* **.NET Framework** — установите [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework) или более поздней версии.

#### <a name="command-examples"></a>Примеры команд
> [!NOTE]
> Так как команды аналитики элементов доступны только в бета-версии, перед их вызовом нужно переключиться на бета-версию профиля.
> ```powershell
>    Select-MgProfile beta
> ```
Чтобы получить конфигурацию аналитики элементов для организации, используйте модуль PowerShell Microsoft Graph и следующую команду, заменив в ней `$TenantId` на идентификатор вашего клиента Azure Active Directory. Этот идентификатор можно получить на странице обзора Azure Active Directory.
```powershell
   Get-MgOrganizationSettingItemInsight -OrganizationId $TenantId
```

По умолчанию аналитика элементов включена для всей организации. С помощью модуля PowerShell Microsoft Graph можно изменить это и отключить аналитику элементов для всех пользователей в организации. 
> [!NOTE]
> Для метода обновления требуются дополнительные разрешения `User.ReadWrite.All`. Чтобы создать сеанс Microsoft Graph с определенной обязательной областью, используйте следующую команду и предоставьте запрошенные разрешения.
> ```powershell
>    Connect-MgGraph -Scopes "User.Read.All","User.ReadWrite.All"
> ```

Используйте следующую команду, заменив `$TenantId` на ваш идентификатор клиента Azure Active Directory и указав для `-IsEnabledInOrganization` значение `false`.
```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $TenantId -IsEnabledInOrganization:$false
```
Также можно изменить поведение по умолчанию и отключить аналитику элементов для определенной группы Azure AD. Используйте следующую команду, заменив `$TenantId` на ваш идентификатор клиента Azure Active Directory, а `$GroupID` — на идентификатор группы Azure Active Directory.
```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $TenantId -DisabledForGroup $GroupId
```

### <a name="configure-item-insights-using-rest-api"></a>Настройка аналитики элементов с помощью API REST
Как сказано выше, параметры конфиденциальности для аналитики элементов по умолчанию включены для всей организации. Эти параметры доступны с помощью свойства навигации с именем **itemInsights** в ресурсе [organizationSettings](/graph/api/resources/organizationsettings?view=graph-rest-beta&preserve-view=true). Параметры по умолчанию можно изменить двумя способами.

- Отключите аналитику элементов для всех пользователей в организации, установив для свойства **isEnabledInOrganization** ресурса [insightsSettings](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) значение `false`. 
- Чтобы отключить элемент insights для _подмножества_ пользователей в группе Azure AD, назначьте этих пользователей в группу Azure AD и задайте для свойства **disabledForGroup** идентификатор этой группы. Узнайте больше о [создании группы и добавлении пользователей в качестве участников](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal). 

Используйте операцию [update](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) для соответствующей настройки свойств **isEnabledInOrganization** и **disabledForGroup**.

| Как включить элемент insights | isEnabledInOrganization | disabledForGroup |
|:-------------|:------------|:------------|
| Вся организация (по умолчанию) | `true` | пусто |
| Недоступно для подмножества пользователей в организации | `true` | Идентификатор группы Azure AD, содержащей подмножество пользователей |
| Недоступно для всей организации | `false` | пропущено |

При обновлении параметров элемента Insights учитывайте следующее:
- [Параметры аналитики](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) доступны только в конечных точках бета-версии.
- Получите идентификатор группы Azure AD на портале Azure и убедитесь в том, что группа существует, так как в ходе обновления не проверяется существование группы. Указание несуществующей группы в **disabledForGroup** _не_ отключает insights для пользователей в организации.
- При изменении параметров в Microsoft 365 новые параметры вступают в силу не сразу: это может занять до 24 часов.
- Независимо от параметров элемента insights, Delve будет по прежнему использовать [настройки конфиденциальности](/sharepoint/delve-for-office-365-admins#control-access-to-delve-and-related-features?view=graph-rest-beta&preserve-view=true) на уровне клиента Delve и пользователя.


## <a name="behavior-changes-in-ui-and-apis"></a>Изменение поведения в пользовательском интерфейсе и интерфейсах API
Полный список затронутых интерфейсов при отключении аналитики элементов см. в статье [Обзор аналитики элементов](item-insights-overview.md#disabling-item-insights). 

## <a name="transition-period"></a>Переходный период
Чтобы настроить параметры элемента Insights, до конца 2020, Microsoft 365 будет использовать и параметры Delve, и параметры элемента insights, и применять более эффективное из них при наличии различий. Это означает, что пользователь считается отказавшимся от использования элемента insights, если он отказался или с помощью элементов управления Delve, или с помощью параметров элемента insights.

По истечении этого переходного периода, настройки Delve применяются только к Delve, а параметры элемента insights влияют только на элемент insights в Microsoft Graph. Убедитесь в том, что вы настроили элемент insights в соответствии с требованиями вашей организации.


> [!NOTE]
> В течение переходного периода, по техническими причинам, стартовая страница SharePoint может предоставлять неактуальные предложения, если в организации отключена аналитика элементов для всех пользователей. Эта проблема будет решена посредством запланированных изменений на стороне сервера. 

## <a name="see-also"></a>См. также
Подробнее о Delve и об использовании параметров Delve для управления отображением документов в канале **Обнаружение**: 
- [Общение и совместная работа в Office Delve](https://support.microsoft.com/office/connect-and-collaborate-in-office-delve-46f92806-b52c-4187-b60e-b3bf8d25f73e)
- [Защищены ли мои документы в Office Delve?](https://support.microsoft.com/office/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3)
- [Delve для администраторов](/sharepoint/delve-for-office-365-admins)
