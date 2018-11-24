# <a name="settings-resource-type"></a>параметры типа ресурсов

Параметры текущего пользователя. Чтобы узнать, как получить или обновить пользовательские параметры, обратитесь к разделу [получить параметры](../api/user_get_settings.md) и [обновление параметров](../api/user_update_settings.md).

Этот ресурс поддерживает:

- Проверка ли пользователь и организации пользователя "участие" для обнаружения контента.
- Отключение и Включение контента обнаружения для определенных пользователей. Кроме того, отключаются документов в Office углубимся.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение параметров пользователя](../api/user_get_settings.md) |[Параметры](../resources/user_settings.md)| Получите параметры пользователей и организаций. |
|[Изменение параметров пользователей](../api/user_update_settings.md) |[Параметры](../resources/user_settings.md)| Обновление текущих параметров пользователя. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Если задано значение true, делегированный доступ для пользователя отключена [прибора](../../beta/resources/insights_trending.md) API. Если параметр имеет значение true, документов в углубимся Office пользователя отключены. Если задано значение true, релевантность содержимое, отображаемое в Office 365, например в предлагаемые сайты в Домашняя страница SharePoint и влияет на представление обнаружения в OneDrive для бизнеса. Пользователи могут управлять этим параметром [Углубимся Office](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Логический|Отражает [уровень организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) управление делегированный доступ, [прибора](../../beta/resources/insights_trending.md) API. Если значение равно true, организации не имеет доступа к углубимся Office. Релевантность содержимое, отображаемое в Office 365, например в предлагаемые сайты в Домашняя страница SharePoint и представления обнаружения в OneDrive для бизнеса контролируется для всей организации. Этот параметр доступен только для чтения и может быть изменено только администраторами в [центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```