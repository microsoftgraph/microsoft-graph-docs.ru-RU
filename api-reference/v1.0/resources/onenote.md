# <a name="onenote-resource-type"></a>Тип ресурса onenote

Точка входа для ресурсов OneNote.

Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

В качестве расположений можно задавать записные книжки пользователя в Office 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Office 365. 

**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a>Авторизация

Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](../../../concepts/permissions_reference.md#notes-permissions).


## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|notebooks|Коллекция [Notebook](notebook.md)|Коллекция записных книжек OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.|
|operations|Коллекция объектов [Operation](onenoteoperation.md) |Состояние операций OneNote. Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`. Только для чтения. Допускается значение null.|
|pages|Коллекция [Page](page.md)|Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.|
|resources|Коллекция объектов [Resource](resource.md) |Изображения и другие ресурсы file на страницах OneNote. Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](resource.md). Только для чтения. Допускается значение null.|
|sectionGroups|Коллекция [SectionGroup](sectiongroup.md)|Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускает значение null.|
|sections|Коллекция [Section](section.md)|Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание записной книжки](../api/onenote_post_notebooks.md) |[Notebook](notebook.md)| Создание записной книжки путем публикации в коллекции записных книжек.|
|[Перечисление записных книжек](../api/onenote_list_notebooks.md) |Коллекция [Notebook](notebook.md)| Получение коллекции записных книжек.|
|[Создание страницы](../api/onenote_post_pages.md) |[Page](page.md)| Создание страницы путем публикации в коллекции страниц.|
|[Перечисление страниц](../api/onenote_list_pages.md) |Коллекция [Page](page.md)| Получение коллекции страниц.|
|[Перечисление групп разделов](../api/onenote_list_sectiongroups.md) |Коллекция [SectionGroup](sectiongroup.md)| Получение коллекции групп разделов.|
|[Перечисление разделов](../api/onenote_list_sections.md) |Коллекция [Section](section.md)| Получение коллекции разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
